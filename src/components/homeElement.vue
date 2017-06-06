<template>
  <div>
    <li class="home-section" v-for="element in elements" :style="{backgroundImage: 'url(' + element.background + ')'}" key="element.id"> 
      <div class="content-wrapper" :style="{color: element.fontColor}"> 
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
  }

  .content-wrapper {
    display: block;
    width: 30%;
    min-width: 370px;
    height: 50vh;
    float: right;
    margin-right: 10%;
    margin-top: 30vh;
  }

  h2 {
    font-family: 'Oswald', sans-serif;
    font-weight: 700;
    color: inherit;
    font-size: 2.5em;
  }
</style>
