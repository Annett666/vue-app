<template>
  <div class="text-block">
    <p class="text-block__title">{{ title }}</p>
    <p class="text-block__subtitle" v-if="subtitle">{{ subtitle }}</p>
  </div>
</template>

<script>
export default {
  name: "TextBlock",
  props: {
    title: String,
    subtitle: String
  }
}
</script>

<style lang="scss" scoped>
.text-block {
  display: flex;
  flex-direction: column;
  row-gap: 8px;
  font-style: normal;
  letter-spacing: 0.02em;

  &__title {
    font-weight: 500;
    font-size: 32px;
    line-height: 48px;
    color: #000000;
  }
  &__subtitle {
    font-weight: 300;
    font-size: 16px;
    line-height: 24px;
    color: #8D8D8D;
  }
}

</style>