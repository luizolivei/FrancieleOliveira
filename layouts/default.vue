<template>
    <div class="content">
      <TopBarDefault class="topBar" style="z-index: 999"/>
      <div style="min-height: 50vh" class="container-layout-default">
        <Nuxt/>
      </div>
      <footer>
        <FooterDefault/>
      </footer>
    </div>
  </template>
  
  <script>
  import TopBarDefault from "../components/layout/TopBar";
  import FooterDefault from "../components/layout/Footer";
  
  export default {
    components: {
        TopBarDefault,
        FooterDefault,
    },
    data() {
      return {
      };
    },
  };
  </script>
  
  <style>
  * {
    box-sizing: border-box;
  }
  
  
  body {
    background: #f4f4f4;
    font-family: Arial, "Helvetica Neue", sans-serif;
  }
  
  .content {
    padding: 0rem;
  }
  
  @media (max-width: 600px) {
    .topBar {
      min-height: auto;
    }
  
    .container-layout-default {
      width: 100%;
      overflow: hidden;
    }
  }
  </style>
  