<template>
  <div>
    <footer>
      <div class="col-left">
        <p><a href="#" class="logo-wrapper"><div class="logo"></div></a></p>
        <p>Copyright &copy; {{ currentYear }} lukaszkups.net</p>
      </div>
      <div class="col-right">
        <p><a href="/home">Home</a></p>
        <p><a href="/home">About</a></p>
        <p><a href="/home">Experience</a></p>
        <p><a href="/home">Projects</a></p>
        <p><a href="/home">Writing</a></p>
      </div>
    </footer>
  </div>
</template>
<script>
  export default {
    computed: {
      currentYear() {
        return new Date().getFullYear();
      }
    }
  }
</script>
<style lang="scss">
  @import './../assets/logo.scss';
  @import './../assets/variables.scss';

  footer {
    font-family: 'Open Sans', sans-serif;
    color: #fff;
    font-size: 0.8em;
    background-color: $dark-color;
    height: 300px;
    padding: 20px;
    margin: 0;
    box-sizing: border-box;
  }

  footer .col-left , footer .col-right{
    display: inline-block;
    margin: 0;
    padding:0;
    width: 45%;
    float: left;
  }

  footer .col-right {
    float: right;
  }

  footer a {
    color: #fff;
  }

  .logo, .logo:before, .logo:after {
    background-color: #fff;
  }

</style>
