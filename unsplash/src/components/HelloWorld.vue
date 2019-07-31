<template>
  <div>
    <h1>{{card}}</h1>
    <h2>{{greet()}}</h2>
    <h2>{{madPeople('miraclelllllll')}}</h2>
    <a :href="joel" >Visit my portfolio</a>
    <div class="grid-gallery active">
      <img width="413" height="270" src="http://placekitten.com/g/413/270" />
      <img width="230" height="200" src="http://placekitten.com/g/230/200" />
      <img width="173" height="153" src="http://placekitten.com/g/173/153" />
      <img width="173" height="440" src="http://placekitten.com/g/173/440" />
      <img width="359" height="235" src="http://placekitten.com/g/359/235" />
      <img width="175" height="125" src="http://placekitten.com/g/175/125" />
      <img width="175" height="125" src="http://placekitten.com/g/175/125" />
      <img width="359" height="125" src="http://placekitten.com/g/359/125" />
      <img width="173" height="328" src="http://placekitten.com/g/173/328" />
      <img width="116" height="104" src="http://placekitten.com/g/116/104" />
      <img width="116" height="104" src="http://placekitten.com/g/116/104" />
      <img width="242" height="210" src="http://placekitten.com/g/242/210" />
    </div>
  </div>
</template>

<script>
// export default {
//   props: ['product'],
//   data () {
//     return {
//       cart: this.$store.state.cart
//     }
//   },
//   computed: {
//     isAdding () {
//       return this.cart.indexOf(this.product) < 0
//     }
//   },
//   methods: {
//     addToCart () {
//       this.$store.commit(ADD_TO_CART, this.product)
//     },
//     removeFromCart (id) {
//       this.$store.commit(REMOVE_FROM_CART, id)
//     }
//   }
// }
export default {
  name: "HelloWorld",
  props: {
    msg: String
  },
  data() {
    return {
      card: "joel",
      joel: "https://ugwumadu116.github.io/joel-ugwumadu/index.html"
    };
  },
  methods: {
    greet: () => {
      return "juninho dey here";
    },
    madPeople: data => {
      return `you type ${data}`;
    }
  }
};
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped>
/* * {
  box-sizing: border-box;
} */

.grid-gallery {
  column-gap: 0.7%;
  display: grid;
  grid-template-columns: 16.42% 12.35% 12.35% 12.5% 12.5% 12.35% 8.28% 8.28%; /*230px 173px 173px 175px 175px 173px 116px 116px*/
  grid-template-rows: 1fr 0.07fr 0.12fr 0.44fr 0.638fr;
  grid-gap: 10px;
  grid-column-gap: 0.7%;
  left: 50%;
  margin: 100px -50vw 0;
  position: relative;
  right: 50%;
  width: 100vw;
}

.grid-gallery img {
  border-radius: 4px;
  height: auto;
  width: 100%;
}

.grid-gallery img:nth-of-type(1) {
  grid-column: 1 / span 2;
  grid-row: 1 / span 3;
}

.grid-gallery img:nth-of-type(2) {
  grid-column: 1;
  grid-row: 4 / span 2;
}

.grid-gallery img:nth-of-type(3) {
  grid-column: 2;
  grid-row: 4 / span 2;
}

.grid-gallery img:nth-of-type(4) {
  align-self: end;
  grid-column: 3;
  grid-row: 1 / span 5;
}

.grid-gallery img:nth-of-type(5) {
  grid-column: 4 / span 2;
  grid-row: 1 / span 2;
}

.grid-gallery img:nth-of-type(6) {
  grid-column: 4;
  grid-row: 3 / span 2;
}

.grid-gallery img:nth-of-type(7) {
  grid-column: 5;
  grid-row: 3 / span 2;
}

.grid-gallery img:nth-of-type(8) {
  grid-column: 4 / span 2;
  grid-row: 5;
}

.grid-gallery img:nth-of-type(9) {
  align-self: center;
  grid-column: 6;
  grid-row: 1 / span 5;
}

.grid-gallery img:nth-of-type(10) {
  align-self: end;
  grid-column: 7;
  grid-row: 1;
}

.grid-gallery img:nth-of-type(11) {
  align-self: end;
  grid-column: 8;
  grid-row: 1;
}

.grid-gallery img:nth-of-type(12) {
  grid-column: 7 / span 2;
  grid-row: 2 / span 4;
}
</style>
