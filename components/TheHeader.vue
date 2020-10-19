<template>
  <div class="columns is-mobile">
    <div class="column is-three-fifths is-offset-one-fifth">
      <nav class="navbar content-center">
        <div id="navbarExampleTransparentExample" class="navbar-menu">
          <div class="navbar-start">
            <nuxt-link to="/" class="navbar-item">
              Home
            </nuxt-link>
            <nuxt-link to="/about" class="navbar-item">
              About Me
            </nuxt-link>
            <nuxt-link to="/work" class="navbar-item">
              Work
            </nuxt-link>
            <nuxt-link to="/site" class="navbar-item">
              This Site
            </nuxt-link>
            <a href="https://github.com/AI1411" target="_blank" class="navbar-item">
              Github
            </a>
          </div>
          <div class="navbar-menu">
            <div class="navbar-end">
              <a href="" class="navbar-item">
                <i class="fab fa-twitter-square fa-2x"></i>
              </a>
              <a href="https://github.com/AI1411" class="navbar-item" target="_blank">
                <i class="fab fa-github fa-2x"></i>
              </a>
            </div>
          </div>
        </div>
      </nav>
    </div>
  </div>

</template>

<script>
export default {
  name: "TheHeader"
}
</script>

<style scoped>
</style>
