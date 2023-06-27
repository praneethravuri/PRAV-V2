<template>
  <div class="section-heading">
    <div class="section-title">
      <p>Experience</p>
    </div>
    <div class="section-line"></div>
  </div>

  <div class="exp-cards">

    <div class="card">
      <div class="card-header">
        <h2 class="card-heading">Software Development Intern @ Cognizant</h2>
      </div>
      <div class="card-location">
        <svg class="location-icon" xmlns="http://www.w3.org/2000/svg" viewBox="0 0 24 24">
          <path
            d="M12 0C7.304 0 3 4.304 3 9c0 1.54.424 2.996 1.155 4.255L12 24l7.845-10.746C20.576 11.996 21 10.54 21 9c0-4.696-4.304-9-9-9zm0 13a3 3 0 100-6 3 3 0 000 6z" />
        </svg>
        <p class="location-text">Hyderabad, India</p>
      </div>
      <p class="card-date">Jan. 2022 - Jun. 2022</p>
      <div class="card-content">
        <p>Developed responsive and user-friendly web application interfaces using front-end technologies and frameworks,
          achieving a remarkable 34% reduction in latency.</p>
        <p>Developed and maintained enterprise web applications, leveraging Restful APIs and CDNs to achieve a notable 30%
          improvement in system performance.</p>
      </div>
    </div>

    <div class="card">
      <div class="card-header">
        <h2 class="card-heading">Frontend Intern @ Stige</h2>
      </div>
      <div class="card-location">
        <svg class="location-icon" xmlns="http://www.w3.org/2000/svg" viewBox="0 0 24 24">
          <path
            d="M12 0C7.304 0 3 4.304 3 9c0 1.54.424 2.996 1.155 4.255L12 24l7.845-10.746C20.576 11.996 21 10.54 21 9c0-4.696-4.304-9-9-9zm0 13a3 3 0 100-6 3 3 0 000 6z" />
        </svg>
        <p class="location-text">Hyderabad, India</p>
      </div>
      <p class="card-date">Aug. 2021 - Oct. 2021</p>
      <div class="card-content">
        <p>Implemented front-end performance optimizations, including lazy loading and code minification, resulting in a
          significant 15% reduction in the website's overall file size</p>
        <p>Collaborated with UX designers to ensure seamless compatibility between design elements and application
          programming interfaces, guaranteeing optimal product functionality.</p>
      </div>
    </div>

    <div class="card">
      <div class="card-header">
        <h2 class="card-heading">Web Developer @ IEEE GRIET SB</h2>
      </div>
      <div class="card-location">
        <svg class="location-icon" xmlns="http://www.w3.org/2000/svg" viewBox="0 0 24 24">
          <path
            d="M12 0C7.304 0 3 4.304 3 9c0 1.54.424 2.996 1.155 4.255L12 24l7.845-10.746C20.576 11.996 21 10.54 21 9c0-4.696-4.304-9-9-9zm0 13a3 3 0 100-6 3 3 0 000 6z" />
        </svg>
        <p class="location-text">Hyderabad, India</p>
      </div>
      <p class="card-date">May. 2019 - May. 2022</p>
      <div class="card-content">
        <p>Headed the IEEE GRIET SB web development team and took charge of the creation, operation, and the maintenance
          of the website</p>
        <p>Selected as the student ambassador for IEEE xTreme 14.0, 2020 competition, responsible for overseeing and
          coordinating all college participants in the hackathon.</p>
      </div>
    </div>

  </div>
</template>


<script>
export default {
  // eslint-disable-next-line vue/multi-word-component-names
  name: "Experience",
}

</script>

<style lang="scss" scoped>
@import "@/styles/_variables.scss";

.exp-cards {
  width: 75%;
  margin: auto;
  margin-top: 20px;
}

.card {
  background-color: $light-navy;
  box-shadow: 0 2px 4px rgba(0, 0, 0, 0.1);
  padding: 20px;
  height: 350px;
  margin: 20px;
  box-shadow: 0 0 10px 0 rgba(0, 0, 0, 0.5);

  &-header {
    display: flex;
    justify-content: space-between;
    align-items: center;
    margin-bottom: 10px;
    padding: 10px 0px;
    border-bottom: 2px solid $dark-red;
  }

  &-heading {
    font-size: 24px;
    font-weight: 600;
    color: $bright-red;
  }

  &-date {
    font-size: 18px;
    color: $silver-sand;
    margin-bottom: 10px;
  }

  &-location {
    display: flex;
    align-items: center;
    margin-bottom: 10px;
  }

  &-content p {
    font-size: 18px;
    margin-bottom: 10px;
    color: $silver-sand;
  }

}

.location {

  &-icon {
    width: 20px;
    height: 20px;
    margin-right: 5px;
    fill: $bright-red;
  }

  &-text {
    font-size: 18px;
    color: $bright-red;
  }
}

@media (max-width: 600px) {
  .exp-cards {
    width: 100%;
  }

  .card {
    padding: 20px;
    width: 100%;
    margin: 15px auto;

    &-heading {
      font-size: 20px;
    }

    &-date,
    &-content p {
      font-size: 14px;
    }
  }

  .location {

    &-icon {
      width: 16px;
      height: 16px;
      margin-right: 3px;
    }

    &-text {
      font-size: 15px;
    }
  }

}</style>