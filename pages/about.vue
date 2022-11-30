<template>
  <div>
    <h2 class="h2">About</h2>
    <p>This strange page holds but a single button. Its true purpose may never be known</p>
    <!-- <div>{{ data }}</div> -->

    <button class="my-7 text-2xl btn" @click="counter++">Add 1</button>
    <p>The button above has been clicked {{ counter }} times. Not that it really matters.</p>
  </div>
</template>

<script>
export default {
data() {
  return {
    counter: 0
  }
}
}

  // const { data } = await useFetch('/api/test')

</script>

<style scoped>

  h2 {
    margin-bottom: 20px;
    font-size: 36px;
  }

  p {
    margin: 20px;
  }
</style>