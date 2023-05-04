<template>
  <div class="home">
    <h1>homePage</h1>
    <p class="red lighten-4 white--text text--darken text--primary text-uppercase">
      Lorem ipsum dolor sit amet, consectetur adipisicing elit. Harum maiores modi quidem veniam, expedita quis laboriosam, ullam facere
      adipisci, iusto, voluptate sapiente corrupti asperiores rem nemo numquam fuga ab at.
    </p>
    <p class="red--text text--lighten-4 font-weight-normal text-center text--primary">
      Lorem ipsum dolor sit amet, consectetur adipisicing elit. Harum maiores modi quidem veniam, expedita quis laboriosam, ullam facere
      adipisci, iusto, voluptate sapiente corrupti asperiores rem nemo numquam fuga ab at.
    </p>
    <p>display</p>
    <!-- 以前是display-1   现在是 text-h1 -->
    <p class="d-1">h1</p>
    <p class="text-h1">h1</p>
    <p class="text-button">button</p>
    <p v-for="item in textList" :class="`text-${item}`">{{ item }}</p>
    <v-icon color="black">mdi-account</v-icon>
  </div>
</template>

<script>
  export default {
    name: 'Home',
    data: () => ({
      textList: ['h1', 'h2', 'h3', 'h4', 'h5', 'h6', 'subtitle1', 'subtitle2', 'body1', 'body2', 'button', 'caption', 'overline'],
    }),
  };
</script>
