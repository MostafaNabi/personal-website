<template>
  <div>
    {{ title }}
  </div>
</template>

<script>
export default {
  name: 'DropdownMenu',
  props: {
    title: {
      required: true,
      type: String
    },
    menu: {
      required: true,
      type: Array
    }
  }
};
</script>

<style lang="scss" scoped>

</style>
