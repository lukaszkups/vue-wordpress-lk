<template>
  <div>
    <div class="main-container">
      <a href="home" class="logo"></a>
      <span class="heading">lukaszkups.net</span>
      <span class="burger"></span>
    </div>
  </div>
</template>
<script></script>
<style lang="scss"> 
  $color: #111;
  $size: 30px;

  .burger, .burger:before, .burger:after{
    width: $size;
    height: 2px;
    background-color: $color;
    display: inline-block;
    margin: 0;
    padding: 0;
    vertical-align: top;
    cursor: pointer;
    float: right;
  }

  .burger:before ,.burger:after{
    content: " ";
  }

  .burger:before {
    margin-top: $size/3;
  }

  .burger:after {
    margin-top: $size/($size/2);
  }
</style>
