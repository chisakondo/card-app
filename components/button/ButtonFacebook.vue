<template>
  <a
    :href="`http://www.facebook.com/share.php?u=${url}`"
    class="py-2 pl-6 relative text-white text-center rounded-md c-button__facebook"
  >
    Facebook
  </a>
</template>

<script>
export default {
  data() {
    return {
      url: "https://profill.ga",
    }
  },
}
</script>

<style scoped>
.c-button__facebook {
  width: 120px;
  background-color: #3b5998;
}

.c-button__facebook:hover {
  background-color: #2d4373;
}

.c-button__facebook::before {
  content: "";
  position: absolute;
  top: 9px;
  left: 10px;
  background-image: url("~assets/images/button/facebook-white.svg");
  background-size: cover;
  height: 22px;
  width: 22px;
  display: inline-block;
}
</style>
