<template>
  <div>
    <vue-cal style="height: 600px" :events="events" />
  </div>
</template>

<script>
import VueCal from "vue-cal";
import "vue-cal/dist/vuecal.css";

export default {
  components: { VueCal },
  data() {
    return {
      events: [
        {
          start: "2024-12-01 10:00",
          end: "2024-12-01 12:00",
          title: "ミーティング",
        },
        {
          start: "2024-12-02 14:00",
          end: "2024-12-02 15:30",
          title: "プレゼン準備",
        },
      ],
    };
  },
};
</script>
