<template>
  <div class="home">
    <sign-in />
  </div>
</template>

<script>
import SignIn from "@/components/home/FrmSignIn.vue";

export default {
  name: "Home",

  components: {
    SignIn,
  },
};
</script>
