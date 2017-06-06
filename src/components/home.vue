<template>
  <div>
    <ul class="home-sections">
      <app-home-element :elements="homeSections"></app-home-element>
    </ul>
  </div>
</template>
<script>
  import HomeElement from './homeElement.vue';

  export default {
    components: {
      appHomeElement: HomeElement
    },
    data() {
      return {
        homeSections: [
          {
            id: 1,
            heading: 'Exploring new horizons of web development',
            background: './dist/static/img/space.jpg',
            body: '<p>I constantly learn latest technologies to provide best services for my clients.</p><p>My current tech stack of choice is:</p><p>Vue.js for the front-end - for delightful experience</p><p>Express.js for the backend - because of versality</p><p>Cordova for mobile - and soon the WEEX</p>',
            fontColor: '#fff'
          },
          {
            id: 2,
            heading: 'Service tailored to Your needs',
            background: './dist/static/img/gears.jpg',
            body: '<p>Every business has its own needs so there\'s a solutions for everyone:</p><p>- Static websites with lifetime support (content updates!),</p><p>- JavaScript development support / outsourcing,</p><p>- Dedicated web applications for the most demanding clients,</p><p>- Hybrid mobile app development</p>',
            fontColor: '#fff'
          },
          {
            id: 3,
            heading: 'In business we trust',
            background: './dist/static/img/cat.jpg',
            body: '<p>This serious cat constantly monitor jira or other task tools to report You about current status anytime.</p><p>Almost 24/7 (naps not included) covered support.</p>',
            fontColor: '#121212'
          },
          
          {
            id: 4,
            heading: 'Ready to work together?',
            background: './dist/static/img/plant.jpg',
            body: '<p><a href="mailto:letstalk@lukaszkups.net">Let\'s be a pair of traditionalists.</a></p><p>Ping me on twitter: <a href="http://twitter.com/lukaszkups">@lukaszkups</a></p>',
            fontColor: '#121212'
          }
        ]
      };
    }
  }  
</script>
<style lang="scss" scoped>
  ul.home-sections {
    margin: 90px 0 0 0;
    padding: 0 20px;
    list-style: none;
    display: block;
    clear:both;
    width: 100%;
    overflow: hidden;
    height: auto;
    min-height: 100%;
    box-sizing: border-box;
  } 
</style>
