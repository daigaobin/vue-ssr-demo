<template>
  <div class="_id">
    动态路由
    {{$route.params.id}}
  </div>
</template>

<script>
  export default {
    name: 'Details',
    validate({params}) {
      // Must be a number
      return /^\d+$/.test(params.id)
    },
    data() {
      return {}
    },
    created() {

    },
    methods: {},
    components: {},
    watch: {}
  }
</script>

<style scoped>
  ._id{
    color: red;
  }
</style>
