<template>
  <div class="flex flex-col justify-center h-screen w-screen items-center" >
    <div class="border-solid border-2 border-black rounded-lg h-2/6 w-4/12 flex justify-center items-center bg-gradient-to-r from-indigo-500 via-purple-500 to-pink-500" >
      <h1 v-if="likes <= 0" class="text-3xl text-white font-bold">
        Nobody likes it
      </h1>
      <h1 class="text-3xl text-white font-bold" v-else>
        This square has {{likes}}
      </h1>
    </div>
    <div >
      <button class="rounded-full bg-blue-500 hover:bg-blue-300 text-white text-2xl w-24 mt-4 w-40" v-on:click="likeSub()">
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