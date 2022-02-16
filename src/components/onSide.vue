<template>
  <div class="onside sticky-top text-plava">
    <img
      class="d-inline mr-1"
      src="@/assets/profiltemplate.png"
      width="64px"
      height="64px"
      alt="your profile picture"
    />
    <p class="d-inline funfont text-ljubicasta">myusername</p>
  </div>
</template>

<script>
export default {
  name: "onSide",
  components: {},
};
</script>
<style scoped>
.onside {
  padding-top: calc(128px + (5vw - 5vh));
}
</style>
