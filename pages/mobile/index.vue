<template>
  <div class="container mx-auto p-5">
    <div class="hidden lg:block mt-32">
      <nav class="flex mb-5" aria-label="Breadcrumb">
        <ol class="inline-flex items-center">
          <li class="inline-flex items-center">
            <a
              href="#"
              class="inline-flex items-center text-sm font-medium text-[#8B96A5] hover:text-blue-600"
            >
              Home
            </a>
          </li>
          <li>
            <div class="flex items-center">
              <svg
                aria-hidden="true"
                class="w-6 h-6 text-gray-400"
                fill="currentColor"
                viewBox="0 0 20 20"
                xmlns="http://www.w3.org/2000/svg"
              >
                <path
                  fill-rule="evenodd"
                  d="M7.293 14.707a1 1 0 010-1.414L10.586 10 7.293 6.707a1 1 0 011.414-1.414l4 4a1 1 0 010 1.414l-4 4a1 1 0 01-1.414 0z"
                  clip-rule="evenodd"
                ></path>
              </svg>
              <a
                href="#"
                class="ml-1 text-sm font-medium text-[#8B96A5] hover:text-blue-600"
                >Clothings</a
              >
            </div>
          </li>
          <li>
            <div class="flex items-center">
              <svg
                aria-hidden="true"
                class="w-6 h-6 text-gray-400"
                fill="currentColor"
                viewBox="0 0 20 20"
                xmlns="http://www.w3.org/2000/svg"
              >
                <path
                  fill-rule="evenodd"
                  d="M7.293 14.707a1 1 0 010-1.414L10.586 10 7.293 6.707a1 1 0 011.414-1.414l4 4a1 1 0 010 1.414l-4 4a1 1 0 01-1.414 0z"
                  clip-rule="evenodd"
                ></path>
              </svg>
              <a
                href="#"
                class="ml-1 text-sm font-medium text-[#8B96A5] hover:text-blue-600"
                >Men’s wear</a
              >
            </div>
          </li>
          <li>
            <div class="flex items-center">
              <svg
                aria-hidden="true"
                class="w-6 h-6 text-gray-400"
                fill="currentColor"
                viewBox="0 0 20 20"
                xmlns="http://www.w3.org/2000/svg"
              >
                <path
                  fill-rule="evenodd"
                  d="M7.293 14.707a1 1 0 010-1.414L10.586 10 7.293 6.707a1 1 0 011.414-1.414l4 4a1 1 0 010 1.414l-4 4a1 1 0 01-1.414 0z"
                  clip-rule="evenodd"
                ></path>
              </svg>
              <a
                href="#"
                class="ml-1 text-sm font-medium text-[#8B96A5] hover:text-blue-600"
                >Summer clothing</a
              >
            </div>
          </li>
        </ol>
      </nav>

      <div class="w-[100%] flex gap-8">
        <Sidebar class="w-[20%]" />

        <div class="w-[80%]">
          <div
            class="border rounded-lg flex items-center justify-between p-4 w-full bg-white mb-5"
          >
            <p>12,911 items in <strong>Mobile accessory</strong></p>
            <div class="flex items-center gap-5">
              <div class="flex items-center gap-3">
                <input type="checkbox" class="w-5 h-5" />
                <span>Verified only</span>
              </div>

              <div class="relative">
                <button
                  @click="toggleMenu"
                  id="dropdownNavbarLink"
                  data-dropdown-toggle="dropdownNavbar"
                  class="flex items-center justify-between rounded-lg border p-2 w-[200px]"
                >
                  Featured
                  <svg
                    class="w-5 h-5 ml-1"
                    aria-hidden="true"
                    fill="currentColor"
                    viewBox="0 0 20 20"
                    xmlns="http://www.w3.org/2000/svg"
                  >
                    <path
                      fill-rule="evenodd"
                      d="M5.293 7.293a1 1 0 011.414 0L10 10.586l3.293-3.293a1 1 0 111.414 1.414l-4 4a1 1 0 01-1.414 0l-4-4a1 1 0 010-1.414z"
                      clip-rule="evenodd"
                    ></path>
                  </svg>
                </button>
                <!-- Dropdown menu -->
                <div
                  id="dropdownNavbar"
                  :class="
                    menu
                      ? 'z-10 absolute font-normal bg-white rounded-b-lg right-0 top-12 w-[200px]'
                      : 'hidden'
                  "
                >
                  <ul
                    class="py-2 text-sm text-gray-900"
                    aria-labelledby="dropdownLargeButton"
                  >
                    <li>
                      <a href="#" class="block px-4 py-2">Nimadur</a>
                    </li>
                    <li>
                      <a href="#" class="block px-4 py-2">Nimadur</a>
                    </li>
                    <li>
                      <a href="#" class="block px-4 py-2">Nimadur</a>
                    </li>
                  </ul>
                </div>
              </div>

              <div class="border rounded-lg flex items-center">
                <button class="bg-[#EFF2F4] text-[25px] p-2 flex items-center">
                  <i class="bx bxs-grid-alt"></i>
                </button>
                <button class="text-[25px] p-2">
                  <i class="bx bx-menu flex items-center"></i>
                </button>
              </div>
            </div>
          </div>

          <div class="flex items-center gap-5 mb-5">
            <button
              class="border border-[rgba(13,110,253,1)] rounded-lg px-2 flex items-center gap-2 text-[#505050] bg-white"
            >
              Samsung <i class="bx bx-x text-[30px] text-[#8B96A5]"></i>
            </button>
            <button
              class="border border-[rgba(13,110,253,1)] rounded-lg px-2 flex items-center gap-2 text-[#505050] bg-white"
            >
              Apple <i class="bx bx-x text-[30px] text-[#8B96A5]"></i>
            </button>
            <button
              class="border border-[rgba(13,110,253,1)] rounded-lg px-2 flex items-center gap-2 text-[#505050] bg-white"
            >
              Poco <i class="bx bx-x text-[30px] text-[#8B96A5]"></i>
            </button>
            <button
              class="border border-[rgba(13,110,253,1)] rounded-lg px-2 flex items-center gap-2 text-[#505050] bg-white"
            >
              Metallic <i class="bx bx-x text-[30px] text-[#8B96A5]"></i>
            </button>
            <button
              class="border border-[rgba(13,110,253,1)] rounded-lg px-2 flex items-center gap-2 text-[#505050] bg-white"
            >
              4 star <i class="bx bx-x text-[30px] text-[#8B96A5]"></i>
            </button>
            <button
              class="border border-[rgba(13,110,253,1)] rounded-lg px-2 flex items-center gap-2 text-[#505050] bg-white"
            >
              3 star <i class="bx bx-x text-[30px] text-[#8B96A5]"></i>
            </button>

            <a href="#" class="text-[#0D6EFD] hover:underline">Clear all filter</a>
          </div>

          <div class="w-[100%] flex flex-wrap gap-[2%]">
            <div
              v-for="mob in mobileLink"
              :key="mob.id"
              class="w-[32%] border rounded-lg bg-white mb-6"
            >
              <div class="flex items-center justify-center border-b py-10">
                <img :src="mob.img" alt="" class="w-[202.4px] h-[202.4px]" />
              </div>
              <div class="flex justify-between px-5 pt-5">
                <div>
                  <h2
                    class="text-[18px] text-[#1C1C1C] font-semibold flex items-center gap-2 mb-1"
                  >
                    {{ mob.price
                    }}<span class="text-[#8B96A5] text-[16px] font-normal">{{
                      mob.oldprice
                    }}</span>
                  </h2>
                  <img src="../../store/img/mobile/rating.png" alt="" />
                </div>
                <button
                  class="px-2 h-10 border rounded-lg flex items-center justify-center"
                >
                  <i class="bx bx-heart text-[25px] text-[#0D6EFD]"></i>
                </button>
              </div>
              <p class="w-[215px] ml-5 my-5">{{ mob.info }}</p>
            </div>
          </div>

          <div class="flex gap-5 float-right">
            <div class="relative">
              <button
                @click="toggleShow"
                id="dropdownNavbarLink"
                data-dropdown-toggle="dropdownNavbar"
                class="flex items-center justify-between rounded-lg border p-2 w-[120px] bg-white"
              >
                Show 10
                <svg
                  class="w-5 h-5 ml-1"
                  aria-hidden="true"
                  fill="currentColor"
                  viewBox="0 0 20 20"
                  xmlns="http://www.w3.org/2000/svg"
                >
                  <path
                    fill-rule="evenodd"
                    d="M5.293 7.293a1 1 0 011.414 0L10 10.586l3.293-3.293a1 1 0 111.414 1.414l-4 4a1 1 0 01-1.414 0l-4-4a1 1 0 010-1.414z"
                    clip-rule="evenodd"
                  ></path>
                </svg>
              </button>
              <!-- Dropdown menu -->
              <div
                id="dropdownNavbar"
                :class="
                  show
                    ? 'z-10 absolute font-normal bg-white rounded-b-lg right-0 top-12 w-full'
                    : 'hidden'
                "
              >
                <ul
                  class="py-2 text-sm text-gray-900"
                  aria-labelledby="dropdownLargeButton"
                >
                  <li>
                    <a href="#" class="block px-4 py-2">20</a>
                  </li>
                  <li>
                    <a href="#" class="block px-4 py-2">30</a>
                  </li>
                  <li>
                    <a href="#" class="block px-4 py-2">40</a>
                  </li>
                </ul>
              </div>
            </div>

            <nav aria-label="Page navigation example">
              <ul class="inline-flex items-center">
                <li>
                  <a
                    href="#"
                    class="block px-3 py-2 ml-0 leading-tight text-gray-500 bg-white border border-gray-300 rounded-l-lg hover:bg-gray-100 hover:text-gray-700"
                  >
                    <span class="sr-only">Previous</span>
                    <svg
                      aria-hidden="true"
                      class="w-5 h-5"
                      fill="currentColor"
                      viewBox="0 0 20 20"
                      xmlns="http://www.w3.org/2000/svg"
                    >
                      <path
                        fill-rule="evenodd"
                        d="M12.707 5.293a1 1 0 010 1.414L9.414 10l3.293 3.293a1 1 0 01-1.414 1.414l-4-4a1 1 0 010-1.414l4-4a1 1 0 011.414 0z"
                        clip-rule="evenodd"
                      ></path>
                    </svg>
                  </a>
                </li>
                <li>
                  <a
                    href="#"
                    class="px-3 py-2 leading-tight text-gray-500 bg-gray-200 border border-gray-300"
                    >1</a
                  >
                </li>
                <li>
                  <a
                    href="#"
                    class="px-3 py-2 leading-tight bg-white border border-gray-300 hover:bg-gray-100 hover:text-gray-700"
                    >2</a
                  >
                </li>
                <li>
                  <a
                    href="#"
                    aria-current="page"
                    class="z-10 px-3 py-2 leading-tight border border-gray-300 bg-white hover:bg-gray-100 hover:text-gray-700"
                    >3</a
                  >
                </li>
                <li>
                  <a
                    href="#"
                    class="block px-3 py-2 leading-tight text-gray-500 bg-white border border-gray-300 rounded-r-lg hover:bg-gray-100 hover:text-gray-70"
                  >
                    <span class="sr-only">Next</span>
                    <svg
                      aria-hidden="true"
                      class="w-5 h-5 text-black"
                      fill="currentColor"
                      viewBox="0 0 20 20"
                      xmlns="http://www.w3.org/2000/svg"
                    >
                      <path
                        fill-rule="evenodd"
                        d="M7.293 14.707a1 1 0 010-1.414L10.586 10 7.293 6.707a1 1 0 011.414-1.414l4 4a1 1 0 010 1.414l-4 4a1 1 0 01-1.414 0z"
                        clip-rule="evenodd"
                      ></path>
                    </svg>
                  </a>
                </li>
              </ul>
            </nav>
          </div>
        </div>
      </div>
    </div>
  </div>

  <!-- Response -->

  <div class="lg:hidden sm:mt-[105px] mt-20 border-b pb-5">
    <div class="container mx-auto px-5">
      <div class="flex flex-wrap items-center gap-3 w-full">
        <button class="text-[#0D6EFD] font-normal bg-[#EFF2F4] py-1.5 px-2 rounded-lg">
          Tablets
        </button>
        <button class="text-[#0D6EFD] font-normal bg-[#EFF2F4] py-1.5 px-2 rounded-lg">
          Phones
        </button>
        <button class="text-[#0D6EFD] font-normal bg-[#EFF2F4] py-1.5 px-2 rounded-lg">
          Ipads
        </button>
        <button class="text-[#0D6EFD] font-normal bg-[#EFF2F4] py-1.5 px-2 rounded-lg">
          Samsung
        </button>
        <button class="text-[#0D6EFD] font-normal bg-[#EFF2F4] py-1.5 px-2 rounded-lg">
          Jackaets
        </button>
        <button class="text-[#0D6EFD] font-normal bg-[#EFF2F4] py-1.5 px-2 rounded-lg">
          Phones
        </button>
        <button class="text-[#0D6EFD] font-normal bg-[#EFF2F4] py-1.5 px-2 rounded-lg">
          Ipads
        </button>
      </div>
    </div>
  </div>

  <div class="lg:hidden container mx-auto px-5 py-3 flex items-center justify-between">
    <button class="border px-2 py-2 rounded-lg flex items-center gap-3">
      <span>Sort: Newest</span> <i class="bx bx-menu-alt-left text-[20px]"></i>
    </button>
    <button class="border px-2 py-2 rounded-lg flex items-center gap-3">
      <span>Filter (3)</span> <i class="bx bx-filter-alt text-[20px]"></i>
    </button>
    <div class="border rounded-lg flex items-center">
      <button class="bg-[#EFF2F4] text-[20px] p-2 flex items-center">
        <i class="bx bxs-grid-alt"></i>
      </button>
      <button class="text-[20px] p-2">
        <i class="bx bx-menu flex items-center"></i>
      </button>
    </div>
  </div>

  <div class="lg:hidden border-t">
    <dir class="container mx-auto px-5 flex flex-wrap items-center gap-5 mb-5">
      <button
        class="border border-[rgba(13,110,253,1)] rounded-lg px-2 flex items-center gap-2 text-[#505050] bg-white"
      >
        Huawei <i class="bx bx-x text-[30px] text-[#8B96A5]"></i>
      </button>
      <button
        class="border border-[rgba(13,110,253,1)] rounded-lg px-2 flex items-center gap-2 text-[#505050] bg-white"
      >
        Apple <i class="bx bx-x text-[30px] text-[#8B96A5]"></i>
      </button>
      <button
        class="border border-[rgba(13,110,253,1)] rounded-lg px-2 flex items-center gap-2 text-[#505050] bg-white"
      >
        64GB <i class="bx bx-x text-[30px] text-[#8B96A5]"></i>
      </button>
    </dir>
  </div>

  <div class="lg:hidden container mx-auto px-5 flex flex-col gap-3 mb-5">
    <div
      v-for="res in resMobLink"
      :key="res.id"
      class="flex items-center border rounded-lg p-5 gap-3 bg-white"
    >
      <img :src="res.img" alt="" class="w-[87.55px] h-[87.55px]" />
      <div>
        <h2 class="text-[#505050] font-normal">Regular Fit Resort Shirt</h2>
        <h3 class="text-[#333333] font-semibold">$57.70</h3>
        <div class="flex items-center gap-5 mt-2">
          <img src="../../store/img/mobile/rating.png" alt="" />
          <p class="text-[#8B96A5] text-[13px] font-normal">154 orders</p>
        </div>
        <p class="text-[#00B517] text-[13px] font-normal">Free Shipping</p>
      </div>
    </div>
  </div>

  <div class="lg:hidden container mx-auto px-5">
    <h2 class="tex-[18px] font-semibold">You may also like</h2>
  </div>

  <div
    class="lg:hidden container mx-auto px-5 flex mb-5 items-center justify-between py-5"
  >
    <button
      @click="back"
      :class="0 == sch ? 'text-gray-200 text-[40px]' : 'text-gray-400 text-[40px]'"
    >
      <i class="bx bxs-chevron-left-circle"></i>
    </button>

    <div class="w-full flex items-center justify-center">
      <div class="flex items-center w-[80%] gap-5">
        <div
          class="flex flex-col justify-center items-center border rounded-lg py-6 w-full bg-white"
        >
          <div class="h-[120px]">
            <img :src="recItemsLink[sch].img" alt="" class="w-[112.27px] h-[113.21px]" />
          </div>
          <div class="flex flex-col items-center gap-2 mt-5">
            <div class="">
              <h2 class="font-medium text-[16px] mb-1">{{ recItemsLink[sch].price }}</h2>
              <p class="text-[#8B96A5] text-[13px] font-normal w-[150px]">
                {{ recItemsLink[sch].info }}
              </p>
            </div>
          </div>
        </div>

        <div
          class="hidden sm:flex flex-col justify-center items-center border rounded-lg py-6 w-full bg-white"
        >
          <div class="h-[120px]">
            <img :src="recItemsLink[sch + 1].img" alt="" class="w-[112.27px] h-[113.21px]" />
          </div>
          <div class="flex flex-col items-center gap-2 mt-5">
            <div class="">
              <h2 class="font-medium text-[16px] mb-1">
                {{ recItemsLink[sch + 1].price }}
              </h2>
              <p class="text-[#8B96A5] text-[13px] font-normal w-[150px]">
                {{ recItemsLink[sch + 1].info }}
              </p>
            </div>
          </div>
        </div>
      </div>
    </div>

    <button
      @click="next"
      :class="
        recItemsLink.length - 2 == sch
          ? 'text-gray-200 text-[40px]'
          : 'text-gray-400 text-[40px]'
      "
    >
      <i class="bx bxs-chevron-right-circle"></i>
    </button>
  </div>
</template>

<script setup>
import { ref } from "vue";
import { mobileLinks } from "../../store/info/mobile";
import { resMobLinks } from "../../store/info/res-mobile";
import { recItemsLinks } from "~/store/info/rec-items";

const resMobLink = ref(resMobLinks);
const mobileLink = ref(mobileLinks);
const recItemsLink = ref(recItemsLinks);

const menu = ref(false);
const toggleMenu = () => (menu.value = !menu.value);

const show = ref(false);
const toggleShow = () => (show.value = !show.value);

const sch = ref(0);
const next = () => {
  if (sch.value == recItemsLink.value.length - 1) {
    sch.value = sch.value;
  } else {
    sch.value = sch.value + 1;
  }
};
const back = () => {
  if (sch.value == 0) {
    sch.value = sch.value;
  } else {
    sch.value = sch.value - 1;
  }
};
</script>

<style lang="scss">
body {
  background-color: #f7fafc;
}
</style>
