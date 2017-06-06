<template>
  <div>
    <div class="header-wrapper">
      <div class="main-container">
        <header>
          <div class="logo-main-wrapper"><a href="home" class="logo-wrapper"><div class="logo"></div></a></div>
          <div class="page-title">lukaszkups.net</div>
          <div class="burger-main-wrapper"><div class="burger-wrapper"><span class="burger"></span></div></div>
        </header>
      </div>
    </div>
  </div>
</template>
<script></script>
<style lang="scss"> 
  @import './../assets/variables.scss';
  @import './../assets/logo.scss';

  $size: 30px;

  .header-wrapper{
    display: block;
    clear: both;
    margin: 0;
    padding: 20px 0;
    background: rgba(250, 250, 250, 0.7);
    position: fixed;
    top: 0;
    left: 0;
    right: 0;
  }

  header {
    display: flex;
    justify-content: space-between;
    width: 100%;
    align-items: center;
  }

  .logo-main-wrapper{
    display: inherit;
    flex: 1 auto;
    width: 50px;
  }

  .page-title {
    font-weight: 100;
    color: $bright-color;
    display: inherit;
    flex: 3 auto;
    letter-spacing: 13px;
    text-transform: uppercase;
    justify-content: center;
    font-family: 'Open Sans', sans-serif;
  }

  .burger-main-wrapper {
    display: inherit;
    flex: 1 auto;
    justify-content: right;
  }

  .burger-wrapper {
    width: 50px;
    height: 50px;
    cursor: pointer;
    text-align:center;
  }
  
  .burger, .burger:before, .burger:after{
    width: $size;
    height: 3px;
    background-color: $color;
    display: inline-block;
    margin: 0;
    padding: 0;
    vertical-align: top;
    float: top;
  }

  .burger {
    margin-top: 15px;
  }

  .burger:before ,.burger:after{
    content: " ";
  }

  .burger:before {
    margin-top: $size/4;
  }

  .burger:after {
    margin-top: -2px;
  }

</style>
