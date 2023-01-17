<template>
  <button :class="mode">
    <slot></slot>
  </button>
</template>
<script>
export default {
  props: ['mode'],
};
</script>

<style scoped>
button {
  padding: 0.75rem 1.5rem;
  font-family: inherit;
  font-weight: bold;
  background-color: #dd6f15;
  border: 1px solid #dd6f15;
  border-radius: 3px;
  color: white;
  cursor: pointer;
}

button:hover,
button:active {
  background-color: #e25f08;
  border-color: #c04f03;
}

.flat {
  background-color: transparent;
  color: #64002fef;
  border: none;
}

.flat:hover,
.flat:active {
  background-color: #e28e1165;
}
</style>
