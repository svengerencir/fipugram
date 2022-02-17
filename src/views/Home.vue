<template>
  <div class="home">
    <div class="row pt-5">
      <div class="col-1 col-md-3"></div>
      <div class="col-7 col-md-4">
        <instagramStory v-for="card in filteredCards" :info="card" />
      </div>
      <div class="col-2 col-md-3">
        <onSide />
      </div>
    </div>
  </div>
</template>

<script>
import instagramStory from "@/components/instagramStory.vue";
import onSide from "@/components/onSide.vue";
import store from "@/store.js";
export default {
  name: "Home",
  data() {
    return {
      cards: [
        {
          storyUser: {
            name: "Mario",
            profile: require("@/assets/prof1.png"),
          },
          storyTitle: "Grize se",
          storyDate: "an hour ago",
          storyPic: "https://picsum.photos/id/1/400/400",
        },
        {
          storyUser: {
            name: "Mtumbu",
            profile: require("@/assets/prof2.png"),
          },
          storyTitle: "Delo delo DELO",
          storyDate: "yesterday",
          storyPic: "https://picsum.photos/id/2/400/400",
        },
        {
          storyUser: {
            name: "Nikola",
            profile: require("@/assets/prof3.png"),
          },
          storyTitle: "Još uvijek dolaze zadaće?",
          storyDate: "two weeks ago",
          storyPic: "https://picsum.photos/id/3/400/400",
        },
      ],
    };
  },
  computed: {
    filteredCards() {
      return this.cards.filter(
        (card) =>
          card.storyTitle
            .toLowerCase()
            .includes(store.searchTerm.toLowerCase()) ||
          card.storyUser.name
            .toLowerCase()
            .includes(store.searchTerm.toLowerCase())
      );
    },
  },
  components: {
    instagramStory,
    onSide,
  },
};
</script>
