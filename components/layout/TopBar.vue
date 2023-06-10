<template>
      <b-navbar toggleable="lg" class="top-bar">
          <b-navbar-nav>
            <b-nav-item href="#sobre">Sobre</b-nav-item>
            <b-nav-item href="/servicos">Serviços</b-nav-item>
            <b-nav-item href="/projetos">Projetos</b-nav-item>
            <b-nav-item href="/social">Social</b-nav-item>
          </b-navbar-nav>
      </b-navbar>
</template>
  
<script>
export default {
  name: 'TopBar'
}
</script>
  
<style scoped>
.top-bar {
  position: fixed;
  width: 100%;
  justify-content: center;
}

.nav-link {
  font-size: 18px;
  text-decoration: underline;
  text-underline-offset: 6px;
}

.navbar-nav {
  flex-direction: row;
}
.nav-item {
  padding: 5px;
}
</style>