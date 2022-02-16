<template>
  <div class="card text-center bg-ljubicasta mt-5">
    <div class="card-header row m-0 p-2">
      <div class="ml-1 mr-auto d-inline-block">
        <img
          class="d-inline"
          src="@/assets/profiltemplate.png"
          width="32px"
          height="32px"
          alt="profile picture"
        />
        <p class="funfont text-white align-middle d-inline">
          &nbsp;someonesUsername
        </p>
      </div>
      <button class="btn text-white btn-naranca rounded-circle">...</button>
    </div>
    <div class="card-body">
      <img class="card-img-top" src="@/assets/kavica.jpg" alt="cup of coffee" />
    </div>
    <div class="card-footer funfont text-naranca">2 days ago</div>
  </div>
</template>

<script>
export default {
  name: "InstagramStory",
  components: {},
};
</script>
<style scoped>
.card-body {
  padding: 0px !important;
}
.card-img-top {
  padding: 0px !important;
}
</style>
