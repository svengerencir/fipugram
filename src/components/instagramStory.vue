<template>
  <div class="card text-center bg-ljubicasta mt-5">
    <div class="text-white funfont text-center d-block pt-2">
      <h4>{{ info.storyTitle }}</h4>
    </div>
    <div class="card-header row m-0 p-2">
      <div class="ml-1 mr-auto d-inline-block">
        <img
          class="d-inline"
          :src="info.storyUser.profile"
          width="32px"
          height="32px"
          alt="profile picture"
        />
        <p class="funfont text-white align-middle d-inline">
          &nbsp;{{ info.storyUser.name }}
        </p>
      </div>
      <button class="btn text-white btn-naranca rounded-circle">...</button>
    </div>
    <div class="card-body m-0 p-0">
      <img class="card-img-top" :src="info.storyPic" alt="cup of coffee" />
    </div>
    <div class="card-footer funfont text-naranca">{{ info.storyDate }}</div>
  </div>
</template>

<script>
export default {
  props: ["info"],
  name: "InstagramStory",
};
</script>
