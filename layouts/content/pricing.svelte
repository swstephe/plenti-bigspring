<script>
  import PricingCard from '../components/pricingCard.svelte';

  export let title, plans, recommended;
</script>

<section class="section pb-0">
  <div class="container text-center">
    <h1 class="display-3">{title}</h1>
  </div>
</section>

<section class="section">
  <div class="container pricing-container">
    <div class="row justify-content-center align-items-center">

    {#each plans as plan}
      {#if plan.recommended === false }
        <div class="col-lg-4 mb-5 mb-lg-0 px-3 pl-3 px-lg-0">
          <div class="card shadow">
            <div class="card-body text-center py-5">

              <PricingCard {...plan}/>

              <a href="/" class="btn btn-outline-primary">Get started for free</a>
            </div>
          </div>
        </div>
      {:else}
        <div class="col-lg-4 col-recommended">
          <div class="card border-0 shadow-lg">
            <div class="card-body text-center py-5">

              <PricingCard {...plan}/>

              <a href="/" class="btn btn-primary">Get started for free</a>
            </div>
          </div>
        </div>
      {/if}
    {/each}

    </div><!-- row -->
  </div><!-- container -->
</section>

<section class="section">
  <div class="container section shadow rounded-lg px-4">
    <div class="row align-items-center justify-content-center text-center text-md-left">
      <div class="col-lg-4 col-md-5 mb-4 mb-md-0">
        <img src="/assets/images/cta.svg" class="img-fluid">
      </div>
      <div class="col-lg-5 col-md-6">
        <h2 class="section-title">Need a larger plan?</h2>
        <p class="mb-4">Lorem ipsum dolor sit amet, consectetur adipiscing elit. Consequat tristique eget amet, tempus eu at consecttur.</p>
        <a href="/contact" class="btn btn-primary">Contact Us</a>
      </div>
    </div>
  </div>
</section>

<style>
  li, .perMonth {
    color:  rgb(119, 119, 119);
  }

  .card-body {
    font-family: lato, sans-serif;
  }

  .display-3 {
    font-size: 3.5rem;
    font-weight: 400;
  }

  .btn-outline-primary {
    background-color: transparent;
    color: #222;
    border-color: transparent;
  }

  .btn-outline-primary::before {
    border-color: #0aa8a7;
  }

  .btn-outline-primary:hover {
    color: #0aa8a7;
  }

  .btn {
    font-size: 16px;
    font-family: lato,sans-serif;
    font-weight: 600;
    text-transform: capitalize;
    padding: 15px 30px;
    border-radius: 30px;
    border: 0;
        border-top-color: currentcolor;
        border-right-color: currentcolor;
        border-bottom-color: currentcolor;
        border-left-color: currentcolor;
    position: relative;
    z-index: 1;
    transition: .2s ease;
    white-space: nowrap;
  }

  .lead {
    font-weight: 400;
    color: #777;
    font-size: 16px;
    line-height: 1.7;
    font-family: lato,sans-serif;

    font-size: 1.25rem;
    font-weight: 400;
  }

  .col-recommended {
    margin: -2rem -1.5rem;
    z-index: 1;
  }

  .col-recommended .btn-primary {
    background-color: #0aa8a7;
    color:  white;
  }

  .price {
    font-size: 50px;
    color: #222;
  }
</style>
