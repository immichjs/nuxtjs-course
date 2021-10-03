<template>
  <div class="flex flex-col justify-center items-center gap-2 mt-4">
    <label>User Id:</label>
    <input type="text" v-model="userId" class="p-2 outline-none ring-2 ring-gray-200 focus:ring-purple-600 transition duration:300 rounded shadow">
    <button @click="onLoadUser" class="bg-purple-400 py-3 px-7 rounded-full hover:bg-purple-600 text-white transition duration-300 shadow-md cursor-pointer font-semibold text-sm">Load User</button>
    <NuxtChild />
  </div>
</template>

<script>
export default {
  layout: 'users',
  data () {
    return {
      userId: ''
    }
  },
  methods: {
    onLoadUser () {
      this.$router.push(`/users/${this.userId}`)
    }
  }
}
</script>
