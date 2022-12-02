<script>
export default {
  data() {
    return {
      socialItems: [
        "../../public/footer-facebook.png",
        "../../public/footer-periscope.png",
        "../../public/footer-pinterest.png",
        "../../public/footer-twitter.png",
        "../../public/footer-youtube.png",
        
      ],
    };
  },
  methods: {},
};
</script>

<template>
  <section>
    <div class="container">
      <div class="d-flex justify-content-between py-5 align-items-center">
        <div class="left-side">
          <button class="btn btn-dark rectangle">SIGN-UP NOW!</button>
        </div>
        <div class="right-side d-flex align-items-center">
          <h4 class="text-primary fw-bold">FOLLOW US</h4>
          <ul class="d-flex gap-3">
            <li v-for="item in socialItems">
              <a href="#">
                <img :src="item" alt="" />
              </a>
            </li>
          </ul>
        </div>
      </div>
    </div>
  </section>
</template>

<style scoped lang="scss">
section {
  background-color: #303030;
}

.rectangle {
  display: flex;
  align-items: center;
  aspect-ratio: 16/6;
  padding: 10px;
  border: 2px solid #157df0;
  color: white;
  font-weight: 800;
  font-size: large;
}

button {
  background-color: transparent;
}
ul {
  list-style: none;
}

.right-side {
  img {
    width: 45px;
  }
}
</style>
