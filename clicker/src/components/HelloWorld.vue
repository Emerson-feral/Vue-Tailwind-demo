<template>
  <div class="flex justify-center h-screen w-screen items-center" >
    <div >
      <h1 v-if="likes <= 0" class="text-3xl text-pink-500 font-bold">
        Nobody likes it
      </h1>
      <h1 class="text-3xl text-green-400 font-bold" v-else>
        This video has {{likes}}
      </h1>
    </div>
    <div >
      <button class="rounded-full bg-blue-500 text-blue-400 text-2xl w-24" v-on:click="likeSub()">
        Like
      </button>
    </div>
  </div>
</template>

<script>
export default {
  data() {
    return {
      likes: 0
    };
  },

  methods: {
    likeSub() {
      this.likes += 1;
    }
  }
};
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped>

  
</style>
