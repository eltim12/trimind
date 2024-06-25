<template>
  <div
    class="trimind-button rounded-pill d-flex align-center justify-center px-6 py-2"
    :class="large ? 'large' : ''"
  >
    {{ text }}
    <img class="ml-1 icon-arrow" src="@/assets/arrow-right.svg" alt="" />
  </div>
</template>
<script setup>
const props = defineProps({
  text: {
    type: String,
    required: true,
  },
  isDark: {
    type: Boolean,
    default: false,
  },
  large: {
    type: Boolean,
    default: false,
  },
});
</script>
<style lang="scss">
.trimind-button {
  background: none;
  border: 1px white solid;
  color: white;
  cursor: pointer;
  transition: transform 0.6s ease, background-color 0.6s ease;
  display: inline-flex;
  align-items: center;
  font-size: 18px;

  &.large {
    padding: 40px 0;
  }

  &:hover {
    background-color: white;
    color: black;

    .icon-arrow {
      filter: invert(0) sepia(1) saturate(10000%) hue-rotate(0deg) brightness(0);
    }
  }

  &:active {
    transform: scale(0.95);
  }
}

.icon-arrow {
  transition: filter 0.6s ease;
}
</style>
