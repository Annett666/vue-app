<template>
  <div class="input-text">
    <label class="input-text__label" for="input">{{ label }}</label>
    <input class="input-text__input" type="text" name="input">
  </div>
</template>

<script>
export default {
  name: "InputText",
  props: {
    label: String
  }
}
</script>

<style lang="scss" scoped>
.input-text {
  margin-bottom: 16px;
  display: flex;
  flex-direction: column;
  row-gap: 8px;
  font-style: normal;
  &__label {
    font-weight: 400;
    font-size: 16px;
    line-height: 24px;
    letter-spacing: 0.02em;
    color: #000000;
  }
  &__input {
    padding: 12px;
    border-width: 0 0 1px;
  }
}
</style>