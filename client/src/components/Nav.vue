<template>

    <nav class="navbar container is-fixed-top is-success" role="navigation" aria-label="main navigation">
        <div class="navbar-brand">
        <a class="navbar-item" href="#">
            <img src="../assets/weight.jpg" height="28">
        </a>

    <a role="button" class="navbar-burger burger" :class="{ 'is-active': isActive}" @click="isActive = !isActive" aria-label="menu" aria-expanded="false" data-target="navbarBasicExample">
      <span aria-hidden="true"></span>
      <span aria-hidden="true"></span>
      <span aria-hidden="true"></span>
    </a>
  </div>

  <div id="navbarBasicExample" class="navbar-menu" :class="{ 'is-active': isActive}">
    <div class="navbar-start">

    <router-link to="/" class="navbar-item">Home</router-link> 
    
    <router-link to="/feed" class="navbar-item">Workout Routine</router-link>

      
      </div>
    </div>

    <div class="navbar-end">
      <div class="navbar-item">
        <LoginBadge />
      </div>
    </div>
  </div>
</nav>
</template>

<script>
import LoginBadge from "@/components/LoginBadge"

export default {
  data: ()=> ({
    isActive: false
  }),
  methods: {},
  components: {
    LoginBadge
  }
}
</script>

<style>

</style>