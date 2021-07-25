<script>
  export let title, body, link, image, background;

  let textPos = 1;
  let textPosMD = 2;
  let imagePos = 2;
  let imagePosMD = 1;
  if (image.position === "right") {
    textPos = 2;
    textPosMD = 1;
    imagePos = 1;
    imagePosMD = 2;
  }

  let backgroundClass = "";
  if (background === "blue") {
    backgroundClass = " bg-light";
  }
</script>

<section class="section{backgroundClass}">
  <div class="container">
    <div class="row align-items-center">

      <div class="col-md-6 order-{textPos} order-md-{textPosMD}">
        <h2 class="section-title">{title}</h2>
        <p>{body}</p>
        <a  href="{link.url}" class="btn-link">
          {link.title}
          <i class="ti-arrow-right"></i>
        </a>
      </div>

      <div class="col-md-6 order-{imagePos} order-md-{imagePosMD} mb-4 mb-md-0">
        <div>
          <img src="/assets/images/{image.url}" alt="{image.alt}" class="img-fluid">
        </div>
      </div>

    </div>
  </div>
</section>

<style>
  .btn-link {
    color: #0aa8a7;
    text-decoration: none;
  }

  .btn-link i {
    font-size: 12px;
    margin-left: 5px;
    transition: .2s ease;
  }

  .btn-link:active i, .btn-link:hover i, .btn-link.focus i, .btn-link.active i {
    margin-left: 10px;
  }
</style>
