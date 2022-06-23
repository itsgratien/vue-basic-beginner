<script setup>
import WelcomeItem from "@/components/WelcomeItem.vue";
</script>

<template>
  <WelcomeItem>
    <h5>John Doe</h5>
    <div>
      <span style="display: block">{{ count }}</span>
      <button type="button" v-on:click="handleCount">count</button>
    </div>
  </WelcomeItem>
</template>

<script>
export default {
  data() {
    return {
      count: 1,
    };
  },
  methods: {
    handleCount(event) {
      event.preventDefault();
      this.count += 1;
    },
  },
};
</script>
