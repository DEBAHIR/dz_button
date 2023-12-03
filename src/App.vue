<template>
  <div>
    <p v-if="age < 18">подросток</p>
    <p v-else-if="age >= 19 && age <= 25">молодой человек</p>
    <p v-else>мужчина</p>
  </div>
</template>

<script>
export default {
  data() {
    return {
      age: 2
    }
  }
}
</script>
