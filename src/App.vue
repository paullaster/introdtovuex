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
    }
  },
  computed: {
    count(){
      return this.$store.state.count;
    }
  },
  methods: {
    counter(){
      this.$store.commit('increment')
    }
  }
}
</script>