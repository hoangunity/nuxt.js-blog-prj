<template>
  <div>
    <TheHeader v-on:sidenavToggle="displaySidenav = !displaySidenav" />
    <TheSidenav
      v-bind:show="displaySidenav"
      v-on:close="displaySidenav = false"
    />
    <Nuxt />
  </div>
</template>

<script>
import TheHeader from "@/components/Navigation/TheHeader";
import TheSidenav from "@/components/Navigation/TheSidenav";

export default {
  components: {
    TheHeader,
    TheSidenav,
  },
  data() {
    return {
      displaySidenav: false,
    };
  },
};
</script>

<style>
html {
  font-family: "Open Sans", sans-serif;
}

body {
  margin: 0;
}
</style>
