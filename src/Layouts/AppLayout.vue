<script setup>
import Header from "@/components/Header.vue";
import Footer from "@/components/Footer.vue";
import home_page from "@/components/home_page.vue";
import { ref } from "vue";

</script>

<template>
  <div class="antialiased bg-white font-sans text-gray-900">

    <Header/>
    <main>
      <slot />
      <home_page/>
      
    </main>
    <Footer/>
  </div>
</template>


