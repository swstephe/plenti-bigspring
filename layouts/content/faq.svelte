<script>
  export let title, questions;
</script>

<section class="section pb-0">
  <div class="container text-center">
    <h1 class="display-3">{title}</h1>
  </div>
</section>

<section class="section">
  <div class="container">
    <div class="row">

      {#each questions as question}
        <div class="col-md-6 mb-4">
          <div class="p-5 shadow rounded-lg">
            <h3 class="mb-4 check-mark">{question.title}</h3>
            <p>{@html question.answer}</p>
          </div>
        </div>
      {/each}

    </div><!-- row -->
  </div><!-- container -->
</section>

<style>
  a.linque {
    text-decoration:  none;
  }

  .display-3 {
    font-size: 3.5rem;
    font-weight: 400;
  }
</style>
