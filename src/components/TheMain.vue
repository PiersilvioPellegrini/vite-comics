<script>
export default {
    data() {
    return {
        itemsList: [
                {
                    img: "buy-comics-digital-comics.png",
                    title: "DIGITAL COMICS",
                },
                {
                    img: "buy-comics-merchandise.png",
                    title: "DC MERCHANDISE",
                },
                {
                    img: "buy-comics-shop-locator.png",
                    title: "SUBSCRIPTION",
                },
                {
                    img: "buy-comics-subscriptions.png",
                    title: "COMIC SHOP LOCATOR",
                },
                {
                    img: "buy-dc-power-visa.svg",
                    title: "DC POWER VISA",
                },
            ],
            

    };
  },
  methods: {
  },
};
</script>

<template>
    <section>
        <div class=" d-flex container px-3 justify-content-between py-5">
            <div v-for="item in itemsList " class="item d-flex align-items-center gap-4 ">
                <img :src ="item.img" alt="">
                <p>{{item.title}}</p> 
            </div>
            
        </div>
    </section>
</template>

<style scoped>
*{
    margin-bottom: 0px;
}
section{
    background-color: #1682F9;
    padding: 20px 0;
}
.item{
    background-color: #1682F9;
    flex-direction: row;
    gap:20px;
    padding:10px 10px;
   
}
img{
    display:block;
    height: 60px;
}

p{
    color:white;
}
</style>
