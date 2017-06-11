<template>
  <div>
    <li class="home-section" v-for="element in elements" :style="{backgroundImage: 'url(' + element.background + ')'}" key="element.id"> 
      <div class="content-wrapper" :style="{color: element.fontColor, background: element.backgroundColor}"> 
        <h2>{{ element.heading }}</h2> 
        <div class="content" v-html="element.body"></div>
      </div>
    </li>
  </div>
</template>
<script>
  export default {
    props: ['elements']
  }
</script>
<style lang="scss" scoped>
  li.home-section {
    list-style: none;
    float: right;
    margin: 0 0 20px 0;
    padding: 0;
    height: 86vh;
    background-size: cover;
    width: 100%;
    display: block;
    filter: grayscale(100%);
  }

  .content-wrapper {
    display: block;
    padding: 20px;
    box-sizing: border-box;
    overflow:hidden;
    width: 30%;
    min-width: 400px;
    height: auto;
    float: right;
    margin-right: 10%;
    margin-top: 25vh;
    border: 2px solid #fff;
  }

  h2 {
    margin-top:0;
    font-family: 'Oswald', sans-serif;
    font-weight: 700;
    color: inherit;
    font-size: 2.5em;
  }
</style>
