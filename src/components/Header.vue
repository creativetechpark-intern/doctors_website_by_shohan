
<script>
import { ref } from 'vue';

export default {
  setup() {
    // States for dropdown and mobile menu
    const isDesktopDropdownOpen = ref(false);
    const isMobileMenuOpen = ref(false);
    const isMobileDropdownOpen = ref(false);

    // Methods to toggle menu states
    const toggleDesktopDropdown = () => {
      isDesktopDropdownOpen.value = !isDesktopDropdownOpen.value;
    };

    const toggleMobileMenu = () => {
      isMobileMenuOpen.value = !isMobileMenuOpen.value;
    };

    const toggleMobileDropdown = () => {
      isMobileDropdownOpen.value = !isMobileDropdownOpen.value;
    };

    // Return values to template
    return {
      isDesktopDropdownOpen,
      isMobileMenuOpen,
      isMobileDropdownOpen,
      toggleDesktopDropdown,
      toggleMobileMenu,
      toggleMobileDropdown
    };
  }
};
</script>





<template>
  <header class="fixed w-full z-50">
    <nav class="bg-blue-600 border-b border-gray-200 shadow-md">
      <div class="container mx-auto px-4 sm:px-6 lg:px-8">
        <div class="flex items-center justify-between h-16">
          <!-- Logo -->
          <div class="flex-shrink-0">
            <a href="/">
              <img src="@/assets/logo.png" alt="Logo" class="h-14" />
            </a>
          </div>

          <!-- Desktop Menu Items -->
          <div class="hidden md:flex space-x-6">
            <a href="/" class="text-white hover:text-blue-200 font-medium">Home</a>

            <!-- Services Dropdown for Desktop -->
            <div class="relative" @click="toggleDesktopDropdown">
              <button class="text-white flex items-center">
                Services
                <svg
                  class="w-4 h-4 ml-1"
                  xmlns="http://www.w3.org/2000/svg"
                  fill="none"
                  viewBox="0 0 24 24"
                  stroke="currentColor"
                >
                  <path stroke-linecap="round" stroke-linejoin="round" stroke-width="2" d="M19 9l-7 7-7-7" />
                </svg>
              </button>

              <!-- Desktop Dropdown Content -->
              <ul v-if="isDesktopDropdownOpen" class="absolute left-0 mt-2 w-48 bg-white shadow-lg rounded-lg z-10 list-none">
                <li><a href="#" class="block px-4 py-2 text-gray-700 hover:bg-gray-100 rounded-md">Clinical Dermatology</a></li>
                <li><a href="#" class="block px-4 py-2 text-gray-700 hover:bg-gray-100">Aesthetic Dermatology</a></li>
                <li><a href="#" class="block px-4 py-2 text-gray-700 hover:bg-gray-100 rounded-md">Dermatologic Surgery</a></li>
                <li><a href="#" class="block px-4 py-2 text-gray-700 hover:bg-gray-100 rounded-md">Cosmetic Dermatology</a></li>
              </ul>
            </div>

            <a href="#about" class="text-white hover:text-blue-200 font-medium">About</a>
            <a href="#contact" class="text-white hover:text-blue-200 font-medium">Contact</a>
          </div>

          <!-- Book Now Button -->
          <div class="hidden md:block">
            <a href="#book" class="px-4 py-2 bg-sky-700 text-white rounded-lg shadow hover:bg-blue-800">Book Now</a>
          </div>

          <!-- Mobile Menu Button -->
          <div class="md:hidden">
            <button @click="toggleMobileMenu" class="text-white focus:outline-none focus:ring-2 focus:ring-blue-500">
              <svg class="h-6 w-6" xmlns="http://www.w3.org/2000/svg" fill="none" viewBox="0 0 24 24" stroke="currentColor">
                <path stroke-linecap="round" stroke-linejoin="round" stroke-width="2" d="M4 6h16M4 12h16m-7 6h7" />
              </svg>
            </button>
          </div>
        </div>
      </div>

      <!-- Mobile Menu -->
      <div v-if="isMobileMenuOpen" class="md:hidden">
        <div class="px-4 py-2 space-y-2 bg-blue-600">
          <a href="/" class="block text-white hover:text-blue-200 font-medium">Home</a>

          <!-- Services Dropdown for Mobile -->
          <div class="relative" @click="toggleMobileDropdown">
            <button class="text-white">Services</button>
            <!-- Mobile Dropdown Content -->
            <ul v-if="isMobileDropdownOpen" class="space-y-2 pt-2 bg-blue-600 list-none">
              <li><a href="#" class="block px-4 py-2 text-white hover:bg-blue-500">Clinical Dermatology</a></li>
              <li><a href="#" class="block px-4 py-2 text-white hover:bg-blue-500">Aesthetic Dermatology</a></li>
              <li><a href="#" class="block px-4 py-2 text-white hover:bg-blue-500">Dermatologic Surgery</a></li>
              <li><a href="#" class="block px-4 py-2 text-white hover:bg-blue-500">Cosmetic Dermatology</a></li>
            </ul>
          </div>

          <a href="#about" class="block text-white hover:text-blue-200 font-medium">About</a>
          <a href="#contact" class="block text-white hover:text-blue-200 font-medium">Contact</a>
          <a href="#book" class="block px-4 py-2 bg-sky-700 text-white rounded-lg shadow hover:bg-blue-800 text-center">Book Now</a>
        </div>
      </div>
    </nav>
  </header>
</template>
