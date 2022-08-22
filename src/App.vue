<template>
  <div>
    <p> count: <strong> {{ count }} </strong></p>
    <button>{{ Increment }}</button>
  </div>
</template>

<script>
export default {
  data(){
    return{
      count: 0,
    }
  }
}

</script>

<style>

</style>