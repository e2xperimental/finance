---
layout: post
title: Share price x Share quantity
date: 2026-11-09 10:00:00 -0000
category: "Calculators"
---

## Share value (price and quantity)

Adjust the starting price, add shares, or change the price increase to see the totals update.

<form id="share-price-calculator" class="share-price-calculator">
  <p>
    <label for="startPrice">Start price</label>
    <input type="number" id="startPrice" name="startPrice" value="217.89" min="0" step="0.01">
  </p>

  <p>
    <label for="shareIncrease">Additional shares: <output id="shareIncreaseValue" for="shareIncrease">0</output></label>
    <input type="range" id="shareIncrease" name="shareIncrease" min="0" max="100" step="1" value="0">
  </p>

  <p>
    <label for="shares">Starting shares</label>
    <input type="number" id="shares" name="shares" value="100" min="0" step="1">
  </p>

  <p>
    <label for="increase">Price increase: <output id="increaseValue" for="increase">0</output>%</label>
    <input type="range" id="increase" name="increase" min="0" max="100" step="1" value="0">
  </p>

  <p>
    <label for="endPrice">End price</label>
    <input type="number" id="endPrice" name="endPrice" readonly>
  </p>

  <p><strong>Starting value:</strong> <output id="startValue">$0.00</output></p>
  <p><strong>Ending value:</strong> <output id="endValue">$0.00</output></p>
</form>

<style>
  .share-price-calculator input[type="number"] { width: 8em; }
  .share-price-calculator input[type="range"] { display: block; width: min(100%, 28rem); }
  .share-price-calculator output { font-variant-numeric: tabular-nums; }
</style>

<script>
  (() => {
    const form = document.getElementById('share-price-calculator');
    if (!form) return;

    const startPrice = form.elements.startPrice;
    const shareIncrease = form.elements.shareIncrease;
    const shares = form.elements.shares;
    const increase = form.elements.increase;
    const endPrice = form.elements.endPrice;
    const money = value => `$${value.toFixed(2)}`;

    function update() {
      const start = Math.max(0, Number(startPrice.value) || 0);
      const quantity = Math.max(0, Number(shares.value) || 0) + Number(shareIncrease.value);
      const end = start * (1 + Number(increase.value) / 100);

      form.querySelector('#shareIncreaseValue').value = shareIncrease.value;
      form.querySelector('#increaseValue').value = increase.value;
      endPrice.value = end.toFixed(2);
      form.querySelector('#startValue').value = money(start * quantity);
      form.querySelector('#endValue').value = money(end * quantity);
    }

    form.addEventListener('input', update);
    update();
  })();
</script>
