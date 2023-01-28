<template>
  <div>
    <button class="button" v-on:click="clickEvent">
      <slot></slot>
      {{ title }}
    </button>
  </div>
</template>

<script>
export default {
  name: "ButtonComponent",
  props: {
    title: String,
    color: String,
    background: String,
    clickEvent: Event
  }
}
</script>

<style scoped>
.button {
  width: 435px;
  height: 65px;
  display: flex;
  align-items: center;
  justify-content: center;
  column-gap: 20px;
  background-color: v-bind(background);
  color: v-bind(color);
  border-radius: 20px;
  font-weight: 500;
  font-size: 20px;
  line-height: 30px;
  letter-spacing: 0.02em;
  cursor: pointer;
}
</style>