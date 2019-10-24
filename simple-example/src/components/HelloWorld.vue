<template>
  <div class="hello_component">

    <h1>{{ message }}, {{ name }}</h1>

    <input type="text" v-model="name" />

    <button class="mono" @click.prevent.stop="clear">clear</button>

  </div>
</template>

<script>
export default {

  props: {
    msg: String
  },

  data() {
    return {
      name: ''
    };
  },

  computed: {
    message() {
      return this.msg.toUpperCase();
    }
  },

  methods: {
    clear() {
      this.name = '';
    }
  }

}
</script>

<style scoped>
  .hello_component > * {
    display: block;
    margin: 1em 0;
  }
</style>
