<template>
  <div v-for="post in posts" :key="post.id">
    <div class="card shadow-sm mb-4">
      <div class="card-body">
        <SinglePost :post="post"></SinglePost>
      </div>
    </div>
  </div>
</template>

<script>
import SinglePost from './SinglePost'
export default {
  components: { SinglePost },
    props:["posts"],
    setup(props){
        console.log(props.posts[0])
    }
}
</script>

<style>

</style>