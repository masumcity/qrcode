<template>
  <div class="container mx-auto">
    <h3>GR Gen</h3>
    <input v-model="qrcode" type="text" class="w-full bg-white rounded border border-gray-300 focus:border-indigo-500 focus:ring-2 focus:ring-indigo-200 text-base outline-none text-gray-700 py-1 px-3 leading-8 transition-colors duration-200 ease-in-out" />
    <hr />

    <qr-code class="mt-5" size="500" :text="qrcode" error-level="H"></qr-code> 
  </div>
</template>

<script>
export default {
  name: "IndexPage",
  data(){
    return {
      qrcode: 'https://google.com'
    }
  }
};
</script>
