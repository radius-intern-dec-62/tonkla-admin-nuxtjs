<template>
  <div class="flex items-center h-screen w-full ">
    <div class="card ">
      <div>
        <h1 class="flex justify-center font-mono mt-10">LOGIN</h1>
      </div>
      <div class="form-login mt-20 ">
        <form class="w-full max-w-sm">
          <t-input-group label="Username " class="font-mono text-base">
            <t-input
              class="w-full focus:outline-none focus:bg-white focus:border-orange-400"
              value=""
              type="Username"
            />
          </t-input-group>

          <t-input-group label="Password" class="mt-10 font-mono ">
            <t-input
              class="w-full focus:outline-none focus:bg-white focus:border-orange-400"
              value=""
              type="password"
            />
          </t-input-group>

          <div class=" flex button mt-10">
            <t-button
              to="/main"
              class="flex w-full justify-center hover:shadow-lg font-mono font-semibold text-white"
              size="lg"
              variant="warning"
              >LOGIN</t-button
            >
          </div>
        </form>
      </div>
    </div>
  </div>
</template>

<style scoped>
.container {
  height: 1500px;
}

.card {
  display: flex;
  width: 500px;
  flex-direction: column;
  background: white;
  height: 580px;
  padding: 40px;
  box-shadow: 0 4px 8px 0 rgba(0, 0, 0, 0.2), 0 6px 20px 0 rgba(0, 0, 0, 0.19);
  border-radius: 10px;
  position: absolute;
  left: 50%;
  top: 50%;
  transform: translate(-50%, -50%);
  /* border: 1px solid; */
}
@media screen and (max-width: 600px) {
  .card {
    width: 100%;
    padding-left: 15px;
    padding-right: 15px;
  }
  .btn-login {
    justify-content: center;
  }
}

/* @media screen and (max-width: 479px) {
  .card {
    width: 100%;
    height: 480px;
    padding-left: 15px;
    padding-right: 15px;
  }
  .btn-login {
    justify-content: center;
  }
} */

/* Extra large devices (large laptops and desktops, 1200px and up) */
.form-login {
  display: flex;
  justify-content: center;
}
</style>
