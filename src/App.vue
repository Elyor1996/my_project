<template>
  <div>
    <p> count: <strong> {{ count }} </strong></p>
    <button class="btn btn-success" v-on:click="increment">Increment</button>
    <button class="btn btn-primary" v-on:click="decrement">Deccrement</button>
  </div>
  <div>
    <div class="comment">
      <div><b>Name:</b> Samar Komilov </div>
      <div><b>Email:</b> samarkomilov@gmail.com </div>
      <div><b>Content:</b> Learn programming </div>
    </div>
    <div class="comment">
      <div><b>Name:</b> Samar Komilov </div>
      <div><b>Email:</b> samarkomilov@gmail.com </div>
      <div><b>Content:</b> Learn programming </div>
    </div>
    <div class="comment">
      <div><b>Name:</b> Samar Komilov </div>
      <div><b>Email:</b> samarkomilov@gmail.com </div>
      <div><b>Content:</b> Learn programming </div>
    </div>
  </div>
</template>

<script>
export default {
  data(){
    return{
      count: 0,

      comments: [
        {id: 1, name: "Elyor", email: "elyor@gmail.com", content: "Learning programming"},
        {id: 1, name: "Elyor", email: "elyor@gmail.com", content: "Learning programming"},
        {id: 1, name: "Elyor", email: "elyor@gmail.com", content: "Learning programming"},
      ]
      }
    },
  methods:{
    increment(){
      this.count +=1
    },
    decrement(){
      this.count -=1
    },

  }
}

</script>

<style>
  .comment{
    border: 3px solid #999;
    padding: 10px;
    margin: 10px;

  }
</style>