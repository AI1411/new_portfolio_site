<template>
  <footer class="footer">
    <div class="content has-text-centered">
      <p>
        <nuxt-link to="/">
          Home
        </nuxt-link>
        <nuxt-link to="/about">
          About Me
        </nuxt-link>
        <nuxt-link to="/work">
          My Work
        </nuxt-link>
        <nuxt-link to="/site">
          This Site
        </nuxt-link>
        <a href="https://github.com/AI1411" target="_blank">
          Github
        </a>
      </p>
    </div>
  </footer>
</template>

<script>
export default {
  name: "TheFooter"
}
</script>

<style scoped>
footer.container{
  max-height: 100px;
}
a {
  padding: 5px;
}
</style>
