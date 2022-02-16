<template>
  <div class="home">
    <div class="row pt-5">
      <div class="col-1 col-md-3"></div>
      <div class="col-7 col-md-4">
        <instagramStory />
        <instagramStory />
        <instagramStory />
      </div>
      <div class="col-2 col-md-3">
        <onSide />
      </div>
    </div>
  </div>
</template>

<script>
import jumbotronHome from "@/components/jumbotronHome.vue";
import instagramStory from "@/components/instagramStory.vue";
import onSide from "@/components/onSide.vue";
export default {
  name: "Home",
  components: {
    jumbotronHome,
    instagramStory,
    onSide,
  },
};
</script>
