<template>
  <div class="header">
    <b-navbar>
      <template slot="brand">
        <b-navbar-item tag="router-link" :to="{ path: '/' }">
          <img
            src="../assets/logo.jpg"
            alt="Material Salon Logo"
          />
        </b-navbar-item>
      </template>
      <template slot="start">
        <b-navbar-item href="#">
          <router-link to="/Page2">About</router-link>
        </b-navbar-item>
        <b-navbar-item href="#">
          <router-link to="/Page3">Services</router-link>
        </b-navbar-item>
        <b-navbar-item href="#">
          <router-link to="/Page4">Team</router-link>
        </b-navbar-item>
        <b-navbar-dropdown label="Info">
          <b-navbar-item href="#">
            About
          </b-navbar-item>
          <b-navbar-item href="#">
            Contact
          </b-navbar-item>
        </b-navbar-dropdown>
      </template>

      <template slot="end">
        <b-navbar-item tag="div">
          <div class="block">
            <a class="button is-light">
              BOOK APPOINTMENT
            </a>
          </div>
        </b-navbar-item>
      </template>
    </b-navbar>
  </div>
</template>

<script>
export default {
  name: "Header",
};
</script>

<style>
.header {
    width: 90%;
    margin: 10px auto;
}

</style>
