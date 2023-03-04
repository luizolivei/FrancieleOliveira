<template>
<b-navbar toggleable="lg" type="dark" variant="info">
    <b-navbar-brand href="#">Meu Site</b-navbar-brand>
    <b-navbar-toggle target="nav-collapse"></b-navbar-toggle>
    <b-collapse id="nav-collapse" is-nav>
      <b-navbar-nav>
        <b-nav-item href="/">Início</b-nav-item>
        <b-nav-item href="/sobre">Sobre</b-nav-item>
        <b-nav-item-dropdown text="Produtos" right>
          <b-dropdown-item href="/produtos/produto1">Produto 1</b-dropdown-item>
          <b-dropdown-item href="/produtos/produto2">Produto 2</b-dropdown-item>
          <b-dropdown-item href="/produtos/produto3">Produto 3</b-dropdown-item>
        </b-nav-item-dropdown>
        <b-nav-item href="/contato">Contato</b-nav-item>
      </b-navbar-nav>
    </b-collapse>
    </b-navbar>
  </template>
  
  <script>
  export default {
    name: 'TopBar'
  }
  </script>
  
  <style scoped>
  </style>