<script>
export default {
  data() {
    return {
      DCComics: [
        "Characters",
        "Comimcs",
        "Movies",
        "Tv",
        "Games",
        "Videos",
        "News",
      ],
      Shop: ["Shop DC", "Shop DC Collectibles"],
      DC: [
        "Terms of Use",
        "Privacy policy(New)",
        "Ad Choices",
        "Advertising",
        "Jobs",
        "Subsciptions",
        "Talent Workshops",
        "CPSC Certificates",
        "Ratings",
        "Shop Help",
        "Contact Us",
      ],
      SITE: [
        "DC",
        "MAD Magazine",
        "DC Kids",
        "DC Universe",
        "DC Power Visa"
      ],
    };
  },
  methods: {},
};
</script>

<template>
  <section class="">
    <div class="container d-flex justify-content-between">
      <div class="left-side d-flex gap-3 py-5">
        <div class="col-5">
          <h3>DC COMICS</h3>
          <ul>
            <li v-for="item in DCComics">{{ item }}</li>
          </ul>
          <h3>Shop</h3>
          <ul>
            <li v-for="item in Shop">{{ item }}</li>
          </ul>
        </div>
        <div class="col-5">
          <h3>DC</h3>
          <ul>
            <li v-for="item in DC">{{ item }}</li>
          </ul>
        </div>
        <div class="col-4">
          <h3>SITE</h3>
          <ul>
            <li v-for="item in SITE">{{ item }}</li>
          </ul>
        </div>
      </div>
      <div class="right-side">
        <img src="../assets/dc-logo-bg.png" alt="">
      </div>
    </div>
  </section>
</template>

<style scoped lang="scss">
section {
  background-image: url(../assets/footer-bg.jpg);
  background-position: center;
  background-repeat: no-repeat;
  background-size: cover;
  color: white;
}
h3 {
  color: white;
  margin-bottom: 20px;
  
}
ul {
  color: grey;
  list-style: none;
  padding-left: 0;
  line-height: 25px;
}

.right-side{
    img{
        width: 915px;
        margin-top: -120px;
        margin-bottom: -100px;
        padding-left: 200px;
        
        
        
    }
}

.container{
    overflow: hidden;
}




</style>
