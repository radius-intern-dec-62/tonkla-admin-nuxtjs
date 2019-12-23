<template>
  <div class="h-screen">
    <div class="grid-container h-full">
      <navbar class="navbar" />
      <div class="sidebar bg-orange-500">
        <div>
          <nuxt-link
            to="/login"
            class="no-underline text-white block text-center mt-10 px-5"
            variant="tertiary"
            >Secondary button</nuxt-link
          >
        </div>
        <div>
          <nuxt-link
            to="/login"
            class="no-underline text-white block text-center mt-10 px-5"
            variant="tertiary"
            >Secondary button</nuxt-link
          >
        </div>
        <div>
          <nuxt-link
            to="/login"
            class="no-underline text-white block text-center mt-10 px-5"
            variant="tertiary"
            >Secondary button</nuxt-link
          >
        </div>
      </div>
      <div class="main text-center">Menu</div>
    </div>
  </div>
</template>

<script>
import navbar from '@/components/navbar'
export default {
  components: {
    navbar
  }
}
</script>

<style scoped>
.grid-container {
  display: grid;
  grid-template-areas:
    'navbar navbar'
    'sidebar main';
  grid-template-columns: auto 1fr;
  grid-template-rows: auto 1fr;
}

.main {
  grid-area: main;
}
.navbar {
  grid-area: navbar;
}
.sidebar {
  display: flex;
  grid-area: sidebar;
  flex-direction: column;
}
</style>
