<template>
  <footer class="hidden lg:block bg-[#EFF2F4] w-full">
    <div class="bg-[#EFF2F4] w-full">
      <div class="container mx-auto px-5">
        <div class="flex flex-col items-center justify-center py-12">
          <h1 class="text-[#1C1C1C] text-[20px]">Subscribe on our newsletter</h1>
          <p class="text-[#606060]">
            Get daily news on upcoming offers from many suppliers all over the world
          </p>
          <div class="flex items-center gap-3 mt-6">
            <div class="relative">
              <i
                class="bx bx-envelope absolute text-[25px] text-[#8B96A5] left-3 top-2"
              ></i>
              <input
                type="text"
                placeholder="Email"
                class="bg-white pl-10 py-2 rounded-lg border outline-none focus:border-[rgba(18,127,255,1)]"
              />
            </div>
            <button class="bg-[rgba(18,127,255,1)] py-2 px-4 rounded-lg text-white">
              Subscribe
            </button>
          </div>
        </div>
      </div>
    </div>

    <div class="bg-white py-10">
      <div class="container mx-auto px-5">
        <div class="flex items-center justify-between">
          <div class="flex flex-col justif-center gap-3">
            <a href="/" class="flex items-center gap-2">
              <img src="../public/favicon.png" alt="" />
              <h1 class="text-[#8CB7F5] text-2xl font-bold">Brand</h1>
            </a>
            <p class="text-[#505050]">
              Best information about the company <br />
              gies here but now lorem ipsum is
            </p>
            <div class="text-[15px] text-white flex items-center gap-3">
              <a href="#"><i class='bx bxl-facebook bg-[#BDC4CD] p-2 rounded-full' ></i></a>
              <a href="#"><i class='bx bxl-twitter bg-[#BDC4CD] p-2 rounded-full' ></i></a>
              <a href="#"><i class='bx bxl-linkedin bg-[#BDC4CD] p-2 rounded-full' ></i></a>
              <a href="#"><i class='bx bxl-instagram bg-[#BDC4CD] p-2 rounded-full' ></i></a>
              <a href="#"><i class='bx bxl-youtube bg-[#BDC4CD] p-2 rounded-full' ></i></a>
            </div>
          </div>

          <div class="flex flex-col justify-center gap-3">
            <h1 class="text-[#1C1C1C]">About</h1>
            <div class="text-[#8B96A5] flex flex-col justify-center gap-1">
              <a href="#" class="hover:underline">About Us</a>
              <a href="#" class="hover:underline">Find store</a>
              <a href="#" class="hover:underline">Categories</a>
              <a href="#" class="hover:underline">Blogs</a>
            </div>
          </div>

          <div class="flex flex-col justify-center gap-3">
            <h1 class="text-[#1C1C1C]">Partnership</h1>
            <div class="text-[#8B96A5] flex flex-col justify-center gap-1">
              <a href="#" class="hover:underline">About Us</a>
              <a href="#" class="hover:underline">Find store</a>
              <a href="#" class="hover:underline">Categories</a>
              <a href="#" class="hover:underline">Blogs</a>
            </div>
          </div>

          <div class="flex flex-col justify-center gap-3">
            <h1 class="text-[#1C1C1C]">Information</h1>
            <div class="text-[#8B96A5] flex flex-col justify-center gap-1">
              <a href="#" class="hover:underline">Help Center</a>
              <a href="#" class="hover:underline">Money Refund</a>
              <a href="#" class="hover:underline">Shipping</a>
              <a href="#" class="hover:underline">Contact us</a>
            </div>
          </div>

          <div class="flex flex-col justify-center gap-3">
            <h1 class="text-[#1C1C1C]">For users</h1>
            <div class="text-[#8B96A5] flex flex-col justify-center gap-1">
              <a href="#" class="hover:underline">Login</a>
              <a href="#" class="hover:underline">Register</a>
              <a href="#" class="hover:underline">Settings</a>
              <a href="#" class="hover:underline">My Orders</a>
            </div>
          </div>

          <div class="flex flex-col justify-center gap-3">
            <h1 class="text-[#1C1C1C]">Get app</h1>
            <div class="flex flex-col justify-center gap-[23px]">
              <button class="bg-[#1C1C1C] rounded-lg px-3 py-2">
                <a href="#">
                  <img src="../store/img/btn-store/app-store.png" alt="" />
                </a>
              </button>

              <button class="bg-[#1C1C1C] rounded-lg px-3 py-2">
                <a href="#">
                  <img src="../store/img/btn-store/google-play.png" alt="" />
                </a>
              </button>
            </div>
          </div>
        </div>
      </div>
    </div>

    <div class="container mx-auto px-5">
      <div class="relative flex items-center justify-between text-[#606060] py-5">
        <p>© 2023 Ecommerce.</p>

        <button
          @click="toggleModal"
          id="dropdownDefaultButton"
          data-dropdown-toggle="dropdown"
          class="text-[#606060] font-medium rounded-lg text-sm px-4 py-2.5 text-center inline-flex gap-1 items-center"
          type="button"
        >
          <img src="../store/img/flag/Property1=US.png" alt="" class="w-[20px]">
          English
          <svg
            class="w-4 h-4 ml-2"
            aria-hidden="true"
            fill="none"
            stroke="currentColor"
            viewBox="0 0 24 24"
            xmlns="http://www.w3.org/2000/svg"
          >
            <path
              stroke-linecap="round"
              stroke-linejoin="round"
              stroke-width="2"
              d="M19 9l-7 7-7-7"
            ></path>
          </svg>
        </button>
        <!-- Dropdown menu -->
        <div
          id="dropdown"
          :class="
            modal
              ? 'absolute z-10 right-0 bottom-14 bg-white  rounded-lg shadow w-44'
              : 'hidden'
          "
        >
          <ul class="py-2 text-sm text-gray-700" aria-labelledby="dropdownDefaultButton">
            <li>
              <a href="#" class="block px-4 py-2 hover:text-blue-500">Russiy</a>
            </li>
            <li>
              <a href="#" class="block px-4 py-2 hover:text-blue-500">Uzbek</a>
            </li>
          </ul>
        </div>
      </div>
    </div>
  </footer>
</template>

<script setup>
import { ref } from "vue";

const modal = ref(false);
const toggleModal = () => (modal.value = !modal.value);
</script>

<style lang="scss" scoped></style>
