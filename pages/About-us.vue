<template>
  <section>
    <section class="jumbotron">
    <div class="row m-0 justify-content-between align-items-end">
      <div class="col-md-6 p-0">
        <h1 class="jumbotron__heading">About Us</h1>
      </div>
    </div>
    </section>
    <section class="section">
      <div class="row m-0 align-items-center justify-content-between">
        <div class="col-md-6 p-0">
          <h2 class="section__heading">About us</h2>
          <p class="section__paragraph">
            With operations starting in Nigeria, our investment portfolio includes leadership, clean energy and power, financial services, agriculture, transport and logistics, and education.
            We understand  that the private sector is the fundamental enabler of economic and social wealth development in Africa, inspires us.
            We invest for the long term, bringing strategic capital, sector expertise, a track record of business turnaround success, and operational excellence to the firms we invest in, all guided by this philosophy.
            Through our initiative; Let’s Use Entrepreneurship initiative, lobbying and research, our initiative program catalyzes entrepreneurship across Africa.
          </p>
        </div>
        <div class="col-md-5 p-0 order-first">
          <p class="section__paragraph">
            <span>We intentional on investing in Africa's most strategic sectors on a long-term basis.</span>
          </p>
        </div>
      </div>
    </section>
    <!-- section class="section section--bg" name="history">
      <div class="row m-0">
        <div class="col-md-7 p-0">
          <h2 class="section__heading">Our history</h2>
          <ul class="timeline">
            <li class="timeline__time" v-for="i in 5" :key="i">
              <h3 class="timeline__heading">2023</h3>
              Lorem ipsum, dolor sit amet consectetur adipisicing elit. Aliquid velit consectetur recusandae officiis sit voluptas laudantium excepturi quidem, quaerat unde!
            </li>
          </ul>
        </div>
      </div>
    </section --->
  <section class="section section--bg">
    <div class="row m-0 justify-content-between align-items-center">
      <div class="col-md-5 p-0">
        <figure class="figure">
          <img src="~/assets/img/David-Utulor.jpg" class="figure__img" alt="Picture of CEO" />
          <figcaption class="figure__caption">
            <h3 class="figure__heading">David Utulor</h3>
            <span>CEO / President</span>
          </figcaption>
        </figure>
      </div>
      <div class="col-md-5 p-0">
        <p class="section__paragraph">
          Our principles are deeply ingrained in our personnel, driving us toward a common goal of creating long-term value for our stakeholders.
        </p>
      </div>
    </div>
    <!--div class="row justify-content-between align-items-center" style="margin: 4rem 0 0;">
      <div class="col-md-3 p-0" v-for="i in 4" :key="i">
        <div class="card card--relative">
          <img src="~/assets/img/David-Utulor.jpg" class="card__img" alt="Picture of CEO" />
          <div class="card__body">
            <h3 class="card__heading">David Utulor</h3>
            <p class="card__heading card__heading--sub">CEO</p>
          </div>
        </div>
      </div>
    </div --->
  </section>
  </section>
</template>

<script>
export default {
  name: 'AboutUsPage'
}
</script>
