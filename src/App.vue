<template>
  <div id="app" class="flyout">
    <navbar dark position="top" class="blue-gradient" scrolling>
      <mdb-navbar-brand href="#/" style="font-weight: bolder;">
        Project Action
      </mdb-navbar-brand>
      <navbar-collapse>
        <navbar-nav left>
          <navbar-item router exact href="/" waves-fixed>Home</navbar-item>
          <navbar-item router href="/upload" waves-fixed>Upload</navbar-item>
          <navbar-item router href="/manage" waves-fixed>Manage</navbar-item>
          <navbar-item router href="/learn" waves-fixed>Learn</navbar-item>
        </navbar-nav>
      </navbar-collapse>
    </navbar>
    <main :style="{marginTop: '60px'}">
      <router-view></router-view>
    </main>
    <Footer color="blue-gradient">
      <p class="footer-copyright mb-0 py-3 text-center">
        &copy; {{new Date().getFullYear()}} Copyright: <a href="#"> Nina Bahler, Johannes Weiß, Christian Schmid,
        Benedikt Seurig </a>
      </p>
    </Footer>
  </div>
</template>

<script>
  import {Navbar, NavbarItem, NavbarNav, NavbarCollapse, mdbNavbarBrand, Footer} from 'mdbvue';

  export default {
    name: 'app',
    components: {
      Navbar,
      NavbarItem,
      NavbarNav,
      NavbarCollapse,
      mdbNavbarBrand,
      Footer
    }
  };

</script>

<style>
  .flyout {
    display: flex;
    flex-direction: column;
    min-height: 100vh;
    justify-content: space-between;
  }

  .active {
    background-color: rgba(255, 255, 255, 0.1);
  }

  .rounded {
    border-radius: 2.125rem !important;
  }

  .label {
    display: inline;
    padding: .2em .6em .3em;
    font-size: 75%;
    font-weight: 700;
    line-height: 1;
    color: #fff;
    text-align: center;
    white-space: nowrap;
    vertical-align: baseline;
    border-radius: .25em;
  }

  .label-info {
    background-color: #5bc0de;
    border-radius: .25em;
  }

  .blue-gradient {
    background: -webkit-linear-gradient(50deg, #45cafc, #303f9f) !important;
    background: -o-linear-gradient(50deg, #45cafc, #303f9f) !important;
    background: linear-gradient(40deg, #45cafc, #303f9f) !important; }

</style>
