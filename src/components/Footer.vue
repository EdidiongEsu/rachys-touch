<template>
  <b-container fluid class="text-center py-5 footer">
    <div class="container-fluid padding">
      <div class="row text-center padding">
        <div class="col-12 social padding">
          <a href="#">
            <i class="fab fa-facebook"></i>
          </a>
          <a href="https://twitter.com/ed_esu">
            <i class="fab fa-twitter"></i>
          </a>
          <a href="#">
            <i class="fab fa-google-plus-g"></i>
          </a>
          <a href="https://www.instagram.com/eddy_esu/">
            <i class="fab fa-instagram"></i>
          </a>
          <a href="#">
            <i class="fab fa-youtube"></i>
          </a>
        </div>
        <div class="col-12">
          <p>
            All right reserved. No part of this website should be copied withut the knowledge of
            the owner or legal counsel. Please, reach out through the contact page for any questions.
          </p>
        </div>
      </div>
    </div>
    <div class="col-12">
      <hr class="mt-2" />
      <div>
        <h5>
          &copy; Rachy'sTouch
          <img src="../assets/images/logo.png" />
        </h5>
      </div>
    </div>
  </b-container>
</template>

<script>
export default {
  name: "Footer",
  data() {},
};
</script>

<style scoped>
.footer {
  background: rgba(212, 210, 210, 0.89);
}
.social a {
  font-size: 30px;
  padding: 17px;
}
.fa-facebook {
  color: #3b5998;
}
.fa-twitter {
  color: #00aced;
}
.fa-google-plus-g {
  color: #dd4b39;
}
.fa-instagram {
  color: #517fa4;
}
.fa-youtube {
  color: #bb0000;
}

.fa-facebook:hover,
.fa-twitter:hover,
.fa-google-plus-g:hover,
.fa-instagram:hover,
.fa-youtube:hover {
  color: #d5d5d5;
}

footer {
  padding-top: 2rem;
}

footer a {
  color: #423c3c;
}
img {
  height: 40px;
}
</style>
