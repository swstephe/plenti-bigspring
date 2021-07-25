<script>
  export let title, price, bestfer, benefits;
</script>

<h3 class="mb-4">{title}</h3>
<span class="price">{price}</span>
<span class="perMonth">/month</span>
<p class="lead">{bestfer}</p>
<ul class="list-unstyled mb-5">
  {#each benefits as benefit}
    <li>{benefit}</li>
  {/each}
</ul>

<style>
  .lead {
    font-weight:  400;
  }

  li, .perMonth {
    color: rgb(119, 119, 119);
  }

  .price {
    font-size: 50px;
    color: #222;
  }
</style>
