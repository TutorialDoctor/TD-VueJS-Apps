<template>
    <div class="base">
        <h1>{{title}}</h1>
        <p>My name is {{name}} and I am {{age}} years old</p>
        <a href="" class="btn btn-warning" v-on:click="greet">Say Hello</a>
        <a href="" class="btn btn-danger" v-on:click="salute">Say Goodbye</a>
    </div><!--end base-->
</template>

<script>
export default {
  name: 'Base',
  props: {
    title: String,
    likes: String,
    isPublished: Boolean,
    CommentIds: Array,
    author: Object,
    callback: Function,
    contactsPromis: Promise //or any other constructor
  },
  data: function(){
    return (
      {
        name:'Base Man',
        age: 0,
      }
    )
  },
  methods:{
    greet: () => alert('Hola!'),
    salute: () => alert('Adios!')
  }
}
</script>

<style scoped>

</style>