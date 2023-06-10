<template>
  <div>
    <select>
      <option value="rice">Rice</option>
      <option value="bread">Bread</option>
    </select>
    <Promotion v-if="showPromote" />
    <button @click="togglePromote">Promote</button>
  </div>
</template>

<script>
import Promotion from "@/components/Promotion.vue";
export default {
  name: "FoodComponent",
  components: {
    Promotion,
  },
  data() {
    return {
      showPromote: false,
    };
  },
  methods: {
    togglePromote() {
      this.showPromote = !this.showPromote;
    },
  },
};
</script>
