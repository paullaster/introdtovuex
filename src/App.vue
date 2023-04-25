<template>
  <div>
    {{count}}
    <button @click="counter">count++</button>
  </div>
</template>
<script>
export default {
  data: function(){
    return {
      count: 0,
    }
  },
  methods: {
    counter(){
      return this.couner = this.count++;
    }
  }
}
</script>