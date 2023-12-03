<template>
  <div>
    <p>{{ text }}</p>
   <button @click="change1">Менять текст</button>
   <button @click="change2">Ага</button>
  </div>
</template>

<style>

</style>

<script>
export default{
  data(){
    return{
      text: 'Привет',
    }
  },
  methods: {
    change1: function() {
      this.text = 'Пока';
    },
    change2: function() {
      this.text = 'Ага'
    }
  }
}
</script>