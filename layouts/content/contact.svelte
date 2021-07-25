<script>
  export let title;
</script>

<section class="section pb-0">
  <div class="container text-center">
    <h1 class="display-3">{title}</h1>
  </div>
</section>

<section class="section bg-white">
  <div class="container">
    <div class="row">
      <div class="col-lg-7 mb-4 mb-lg-0">
        <form action="#" method="POST">
          <input type="text" class="form-control mb-3" id="name" name="name" placeholder="Your Name">
          <input type="email" class="form-control mb-3" id="mail" name="mail" placeholder="Your Email">
          <input type="text" class="form-control mb-3" id="subject" name="subject" placeholder="Subject">
          <textarea name="message" id="message" class="form-control mb-3" placeholder="Your Message"></textarea>
          <button type="submit" value="send" class="btn btn-primary">Send Now</button>
        </form>
      </div>

      <div class="col-lg-5 content">
        <h3 id="why-you-should-contact-us">Why you should contact us!</h3>
        <p>
          Lorem ipsum dolor sit amet, consectetur adipisicing elit. Velit recusandae voluptates doloremque veniam temporibus porro culpa ipsa, nisi soluta minima saepe laboriosam debitis nesciunt.
        </p>
        <ul>
        <li><strong>Phone: +88 125 256 452</strong></li>
        <li><strong>Mail: <a href="mailto:info@bigspring.com">info@bigspring.com</a></strong></li>
        <li><strong>Address: 360 Main rd, Rio, Brazil</strong></li>
        </ul>
      </div>

    </div>
  </div>
</section>

<style>
  h3, .h3 {
    font-size: 24px;
  }

  .display-3 {
    font-size: 3.5rem;
    font-weight: 400;
  }

  .content ul {
    list-style-type: none;
  }

  .content ul li {
    padding-left: 20px;
    position: relative;
    color:  rgb(119, 119, 119);
  }

  li::before {
    position: absolute;
    content: '';
    height: 8px;
    width: 8px;
    border-radius: 50%;
    background: #0aa8a7;
    left: 3px;
    top: 5px;
  }

  .content strong {
    font-weight: 600;
  }

  li a {
    color:  rgb(119, 119, 119);
  }

  li a:hover {
    color: #0aa8a7;
    text-decoration: none;
  }
</style>
