<template>
  <div>
    <nav class="flex items-center justify-between flex-wrap bg-orange-500 p-6">
      <div class="flex items-center flex-shrink-0 text-white mr-6">
        <svg
          class="fill-current h-8 w-8 mr-2"
          width="54"
          height="54"
          viewBox="0 0 54 54"
          xmlns="http://www.w3.org/2000/svg"
        >
          <path
            d="M13.5 22.1c1.8-7.2 6.3-10.8 13.5-10.8 10.8 0 12.15 8.1 17.55 9.45 3.6.9 6.75-.45 9.45-4.05-1.8 7.2-6.3 10.8-13.5 10.8-10.8 0-12.15-8.1-17.55-9.45-3.6-.9-6.75.45-9.45 4.05zM0 38.3c1.8-7.2 6.3-10.8 13.5-10.8 10.8 0 12.15 8.1 17.55 9.45 3.6.9 6.75-.45 9.45-4.05-1.8 7.2-6.3 10.8-13.5 10.8-10.8 0-12.15-8.1-17.55-9.45-3.6-.9-6.75.45-9.45 4.05z"
          />
        </svg>
        <span class="font-semibold text-xl tracking-tight">TONKLA</span>
      </div>
      <div class="block lg:hidden">
        <button
          class="flex items-center px-3 py-2 border rounded text-teal-200 border-teal-400 hover:text-white hover:border-white"
        >
          <svg
            class="fill-current h-3 w-3"
            viewBox="0 0 20 20"
            xmlns="http://www.w3.org/2000/svg"
          >
            <title>Menu</title>
            <path d="M0 3h20v2H0V3zm0 6h20v2H0V9zm0 6h20v2H0v-2z" />
          </svg>
        </button>
      </div>

      <div class="w-full  justify-end lg:flex lg:items-center lg:w-auto ">
        <t-dropdown
          text="Account"
          placement="bottom-end"
          class="w-auto border-none"
        >
          <div>
            <nuxt-link
              to="/login"
              class="block no-underline px-4 py-2 hover:bg-grey-600 hover:text-white text-black px-6 m-3 rounded  "
              variant="tertiary"
              >My Profile</nuxt-link
            >
          </div>
          <div class="  ">
            <nuxt-link
              to="/login"
              class="block no-underline px-4 py-2 hover:bg-grey-600 hover:text-white text-black px-6 m-3"
              variant="tertiary"
              >Setting</nuxt-link
            >
          </div>
          <div>
            <nuxt-link
              to="/login"
              class="block no-underline px-4 py-2 hover:bg-grey-600 hover:text-white text-black px-6 m-3"
              variant="tertiary"
              >Logout</nuxt-link
            >
          </div>
        </t-dropdown>
      </div>
    </nav>
  </div>
</template>

<script>
export default {
  data() {
    return {
      toggle: false
    }
  }
}
</script>

<style scoped>
/* .useracount {
  height: 250px;
  width: 300px;
  position: absolute;
  display: flex;
  justify-content: flex-start;
  transform: translate3d(-220px, 0px, 0px);
  background: white;
  box-shadow: 0 4px 8px 0 rgba(0, 0, 0, 0.2), 0 6px 20px 0 rgba(0, 0, 0, 0.19);
  border-radius: 10px;
} */
/* .usersetting {
  flex-direction: column;
  text-align: center;
} */
</style>
