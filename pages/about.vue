<template>
  <div>
    <h2 class="h2">About</h2>
    <p class="pOne">This strange page holds but a single button. Its true purpose may never be known.</p>
    <!-- <div>{{ data }}</div> -->

    <button class="my-7 text-2xl btn" @click="counter++">Add 1</button>
    <p class="pTwo">The button above has been clicked <strong>{{ counter }}</strong> times. <em>Not that it really matters.</em></p>
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

  .pOne {
    text-align: center;
    margin: auto;
    margin-top: 50px;
    margin-bottom: 20px;
    font-size: 2rem;
  }

  .pTwo {
    text-align: center;
    margin: auto;
    margin-top: 20px;
    font-size: 2rem;
  }

  .btn {
    display: block;
    margin: auto;
    font-size: 4rem;
    padding: 40px;
  }
</style>