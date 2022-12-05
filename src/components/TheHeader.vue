<script>
// importo l'array
import { cardsItems } from "../composable/cardItems";
export default {
  data() {
    return {
      cardsItems: cardsItems,
    };
  },
  methods: {},
};
</script>

<template>
  <section class="bg-black">
    <div class="container pb-5">
      <div class="subtitle">
        <h2>CURRENT SERIES</h2>
      </div>
      <div class="cards">
        <!-- ciclo sulla nuova varibaile che prende il valore dell'array importato -->
        <div v-for="cardItem in cardsItems" class="col-2 cardItem d-flex-row">
          <div class="cardImg">
            <img :src="cardItem.thumb" alt="" />
          </div>
          <div class="cardTitle">{{ cardItem.series }}</div>
        </div>
      </div>
    </div>
  </section>
</template>

<style scoped lang="scss">
.subtitle {
  background-color: #157df0;
  color: white;
  width: fit-content;
  padding: 10px 40px;
  position: relative;
  z-index: 10;
  top: -30px;

  h3 {
    font-weight: 700;
  }
}
.cards {
  display: flex;
  flex-wrap: wrap;
}
.cardItem {
  padding: 10px 20px;
  color: white;

  .cardImg {
    img {
      aspect-ratio: 1/1;
      display: block;
      height: 100%;
      width: 100%;
      object-fit: cover;
      object-position: top;
    }
  }

  .cardTitle {
    padding-top: 20px;
    font-weight: 400;
    font-size: 16px;
  }
}
</style>
