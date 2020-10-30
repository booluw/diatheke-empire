<template>
  <main>
    <career-jumbotron />
    <section class="section section--w-60">
      <h3 class="heading heading--sub">LIFE AT DIATHEKE</h3>
      <p class="paragraph">
        Here everyone matters and we are committed to mutual development. We believe in an inclusive system of operation where dignity, peculiarity and opinion of every individual is highly respected.
        We see each other as family, hence our determination to add value to one another.
        <br /><br />
        In Diatheke, everyone is a leader and WE all make up te full Diatheke story.
      </p>
    </section>
    <section class="section section--w-60">
      <h3 class="heading heading--sub">careers</h3>
      <p class="paragraph">
        In line with our development strategy, our employees are exposed to tailored trainings, mentorship and coaching fashioned to
        individual need and requirement, to help them improve their skills and to be better equipped even in more challenging roles.
        With our defined career growth model, you are sure to transcend with greater opportunities.
      </p>
    </section>
    <section class="section section--w-60">
      <h3 class="heading heading--sub">Welfare</h3>
      <p class="paragraph">
        The well-being of our employees is of great value to us. This is part of our core values. We have well structured compensation packages, competitive salary and other related baseline packages.
        Our welfare and reward structure is ever evolving and captures more broad perspectives. We believe the more we grow the better YOU become.
      </p>
    </section>
    <div class="row row--align-center row--justify-spaced section" style="background-color: #ed3237">
      <div class="col-3">
        <section class="section section--npad">
          <h3 class="heading heading--sub" style="color: white;">Organisation</h3>
          <p class="paragraph">
            Our mode of operation drives everyone to be more creative in their thinking, innovative in their operation and expressive in their participation to push the growth of the empire
            in developing solutions for our nation, continent and the world at large.
          </p>
          <br />
          <p class="paragraph">
            As an empire, we are responsible for setting the pace for exceptional corporate values and ethics, which is the foundation of our organisation.
          </p>
        </section>
      </div>
      <div class="col-2">
        <img src="~/assets/img/favicon.png" style="width: 100%;" />
      </div>
    </div>
    <section class="section section--w-60">
      <h3 class="heading heading--sub">Jobs</h3>
      <p class="paragraph">
        Diatheke Empire has a distinctive and ambitious mission: <i>improving livelihood, through regeneration of capital and distribution of resources for a stable economy.</i>
        As we challenge you to embark on your journey of achieving greatness and breaking boundaries, have goals at heart because it comes with fulfilling and sublime rewards.
      </p>
    </section>
    <section class="section section--w-60">
      <h3 class="heading heading--sub">People</h3>
      <p class="paragraph">
        Diatheke Empire provides opportunities to wide range of talented and ambitious professionals to become a part of a greater whole, working to transform Africa. Do you have
        a desire to be part of the change agents? We are keen to meet you.
        <br /><br />
        If you're intrested in any future positions or vacancies, please send an email to <b>careers@diathekeempire.com</b>.
      </p>
    </section>
    <section class="section">
      <h2 class="heading heading--sub">
        The Diatheke Empire Creed
      </h2>
      <p class="paragraph paragraph--w-60">
        These values stem from our Founder's beliefs, practices and culture; philosophies that have been tested and proven
        over time to bring out the best in us.
      </p>
      <div class="row row--mt2">
        <div class="col-2">
          <div class="card">
            <div class="card__big-text">E</div>
            <h3 class="card__heading">Excellence</h3>
            <p class="card__text">
              To be an exceptional company, where every product is at it's peak efficiency and provides it's maximum satisfaction.
            </p>
          </div>
        </div>
        <div class="col-2">
          <div class="card">
            <div class="card__big-text">I</div>
            <h3 class="card__heading">Integrity</h3>
            <p class="card__text">
              Upholding honesty and strong moral principles towards our investments and consumers to enhance stronger relationships.
            </p>
          </div>
        </div>
        <div class="col-2">
          <div class="card">
            <div class="card__big-text">I</div>
            <h3 class="card__heading">Innovation</h3>
            <p class="card__text">
              To create extraordinary products with a blend of creativity, modern ideas and new innovation that will standout among others.
            </p>
          </div>
        </div>
      </div>
    </section>
    <section class="section section--w-60">
      <h3 class="heading heading--sub">Fraud</h3>
      <p class="paragraph">
        Several incidents involving organisations and individuals fraudulently claiming to recruit on behalf of Diatheke Empire have never occurred.
        <br /><br />
        The scammers' goal is to extort money from candidates by asking for payment upfront for fake ancillary costs (travel agency, visa fees, e.t.c) or to obtain personal and financial information
        (bank account details, personal address, e.t.c).
        <br /><br />
        But be adviced that Diatheke Empire, its subsidiaries or any organisation working on behalf of the empire for recruitment purposes will never request payment nor will it ask for financial information
        during the recruitment and selection process.
        <br /><br />
        We take this situation very seriously and implement all possible measures to identify and stop this type of fraud.
      </p>
    </section>
    <section class="section section--w-60">
      <h3 class="heading heading--sub">Prevention tips</h3>
      <p class="paragraph">
        Please find below some prevention tips that you should keep in mind:
      </p>
      <ul class="section__list">
        <li>Consult and apply for jobs opportunities on our dedicated recruitment webpage: https://diathekeempire.com/careers</li>
        <li>Do not disclose personal or financial information to an unknown party.</li>
        <li>Do not respond to unsolicited or suspicious job offers. Confirm all jobs from our website and apply only through the designated channels.</li>
      </ul>
    </section>
  </main>
</template>

<script>
import CareerJumbotronVue from '~/components/CareerJumbotron.vue'
export default {
  name: 'CareerVue',
  components: {
    'career-jumbotron': CareerJumbotronVue
  }
}
</script>

<style>

</style>