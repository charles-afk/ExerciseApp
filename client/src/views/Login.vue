<template>
<div class="level section">

<div class="level-item">

<form style="padding-top: 60px;">
  <div class="field">
  <p class="control has-icons-left has-icons-right">
    <input class="input" type="email" placeholder="Email">
    <span class="icon is-small is-left">
      <i class="fas fa-envelope"></i>
    </span>
    <span class="icon is-small is-right">
      <i class="fas fa-check"></i>
    </span>
  </p>
</div>
<div class="field">
  <p class="control has-icons-left">
    <input class="input" type="password" placeholder="Password">
    <span class="icon is-small is-left">
      <i class="fas fa-lock"></i>
    </span>
  </p>
</div>
<div class="field">
  <p class="control">
    <button class="button is-success" @click.prevent="login">
      Login
    </button>
  </p>
</div>
</form>
</div>
</div>
</template>

<script>
import session from "@/models/session";

export default {
  methods: {
    login(){
      session.user = {
        name:'Charles Agudelo',
        handle:'charles-afk',
        profile:''
      }
      this.$router.push('feed')
    }
  }
}
</script>

<style>

</style>