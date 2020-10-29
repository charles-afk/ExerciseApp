<template>
  <div class="page" style="padding-top: 60px;">
      <h2 class="title is-2">Workout Routine!</h2>

        <div class="columns">
          <div class="column is-one-quarter">
              <Sidebar />
          </div>
          <div class="column is-three-quarters">
              <Post />
          </div>  
        </div>
  </div>
</template>

<script>
import Sidebar from "@/components/Sidebar"
import Post from "@/components/Post"
import {posts} from "@/models/feed"

export default {
    data(){
        return {
            posts
        }
    },
    components: {
        Sidebar, Post
    }
}
</script>

<style>
  .card {
    margin-bottom: 15px;
  }
</style>>