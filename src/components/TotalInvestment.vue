<template>
<div class="main">
<p class="hello"><b>Hello Basil</b></p>
<p style="margin-bottom: 15px;">Here's your investment overview</p>
<div class="totalinv">
<div class="box" style="background-color: #fff">
<div class="shift-small">
<p style="color: #555; font-size:11px;">Total Investment</p>
<h3 style="color: black">₦110,000.00</h3>
</div>
<div class="shifter shift-small">
<p style="color: #555; font-size:11px;">Return On Investment</p>
<h3 style="color: black;">₦5,000.00</h3>
</div>
</div>
<div class="boxx b" style="background-color: #222">
<div class="shift-small">
<p style="color: #888; font-size:11px;">Wallet Balance</p>
<h3 style="color: white">₦70,000.00</h3>
</div>
<div class="money">
<p><i style="color:lightgreen;" class="fas fa-envelope"></i></p>
</div>
</div>
</div>
</div>
</template>

<script>
export default {
  name: 'TotalInvestment'
}
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
