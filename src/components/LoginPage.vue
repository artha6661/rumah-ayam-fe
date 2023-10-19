<!-- Login.vue -->
<template>
    <div class="min-h-screen flex items-center justify-center bg-gray-100">
      <div class="bg-white p-8 rounded-lg shadow-md w-full max-w-md">
        <h2 class="text-2xl font-semibold mb-6 text-gray-800">Login</h2>
        <form @submit.prevent="login">
          <div class="mb-4">
            <label for="email" class="block text-gray-600 font-medium">Email</label>
            <input
              type="email"
              id="email"
              v-model="email"
              class="w-full mt-1 p-2 rounded border border-gray-300 focus:outline-none focus:border-indigo-500"
              required
            />
          </div>
          <div class="mb-4">
            <label for="password" class="block text-gray-600 font-medium">Password</label>
            <input
              type="password"
              id="password"
              v-model="password"
              class="w-full mt-1 p-2 rounded border border-gray-300 focus:outline-none focus:border-indigo-500"
              required
            />
          </div>
          <div class="mb-4">
            <button
              type="submit"
              class="w-full py-2 px-4 bg-indigo-500 text-white font-semibold rounded hover:bg-indigo-600 focus:outline-none"
            >
              Login
            </button>
          </div>
        </form>
      </div>
    </div>
  </template>
  
  <script>
  export default {
    data() {
      return {
        email: '',
        password: '',
      };
    },
    methods: {
      login() {
        // Add your login logic here
        // You can use this.email and this.password to access user input
      },
    },
  };
  </script>
  
  <style>
  /* You can add custom styles here if needed */
  </style>
  