<template>
  <Magnetisme />
  <Reiki />
</template>

<script>
import Magnetisme from "@/components/Magnetisme.vue";
import Reiki from "@/components/Reiki.vue";
export default {
  name: "SoinsDesktop",
  components: {
    Magnetisme,
    Reiki,
  },
  data() {
    return {
      seeMore: null,
    };
  },
};
</script>
