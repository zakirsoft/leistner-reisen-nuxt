<template>
  <!-- Header  -->
  <header>
    <div class="header-logo">
      <div class="container">
        <div class="top-logo">
          <a href="#" class="logo">
            <img src="~/assets/images/logo.png" alt="">
          </a>
        </div>
      </div>
    </div>
    <nav id="desktopNav">
      <div class="container">
        <div class="main-menu">
          <ul>
            <li>
              <a href="#"> Home </a>
            </li>
            <li>
              <a href="#"> Reisen </a>
            </li>
            <li>
              <a href="#"> Service & Info </a>
            </li>
            <li>
              <a href="#"> Unternehmen </a>
            </li>
            <li>
              <a href="#"> Busanmietung </a>
            </li>
            <li>
              <a href="#"> Kontakt </a>
            </li>
          </ul>
        </div>
      </div>
    </nav>
    <nav id="mobileNav">
      <div class="toggle-button" @click="mobileMenu = !mobileMenu">
        <div class="text">
          Menu
        </div>
        <div class="icon">
          <svg
            v-if="!mobileMenu"
            xmlns="http://www.w3.org/2000/svg"
            width="24"
            height="24"
            viewBox="0 0 24 24"
            fill="none"
            stroke="currentColor"
            stroke-width="2"
            stroke-linecap="round"
            stroke-linejoin="round"
            class="feather feather-menu"
          ><line x1="3" y1="12" x2="21" y2="12" /><line x1="3" y1="6" x2="21" y2="6" /><line x1="3" y1="18" x2="21" y2="18" /></svg>
          <svg
            v-else
            xmlns="http://www.w3.org/2000/svg"
            width="24"
            height="24"
            viewBox="0 0 24 24"
            fill="none"
            stroke="currentColor"
            stroke-width="2"
            stroke-linecap="round"
            stroke-linejoin="round"
            class="feather feather-x"
          ><line x1="18" y1="6" x2="6" y2="18" /><line x1="6" y1="6" x2="18" y2="18" /></svg>
        </div>
      </div>
      <ul :class="{ 'active': mobileMenu }">
        <li> <a href="#"> Home </a> </li>
        <li> <a href="#"> Reisen </a> </li>
        <li> <a href="#"> Service & Info </a> </li>
        <li> <a href="#"> Unternehmen </a> </li>
        <li> <a href="#"> Busanmietung </a> </li>
        <li> <a href="#"> Kontakt </a> </li>
      </ul>
    </nav>
  </header>
</template>

<script>
export default {
  data () {
    return {
      mobileMenu: false
    }
  }
}
</script>

<style>

</style>
