<template>
  <header class="fixed z-50 w-full top-0">
    <div class="bg-white border-gray-200 border-b">
      <div class="container mx-auto px-5">
        <nav class="py-2.5">
          <div class="flex flex-wrap justify-between items-center">
            <div class="flex item-center justify-between gap-3">
              <div class="flex items-center lg:order-2 lg:hidden">
                <button
                @click="toggleModal"
                  data-collapse-toggle="mobile-menu-2"
                  type="button"
                  class="inline-flex items-center text-sm text-gray-500"
                  aria-controls="mobile-menu-2"
                  aria-expanded="false"
                >
                  <span class="sr-only">Open main menu</span>
                  <svg
                    class="w-6 h-6"
                    fill="currentColor"
                    viewBox="0 0 20 20"
                    xmlns="http://www.w3.org/2000/svg"
                  >
                    <path
                      fill-rule="evenodd"
                      d="M3 5a1 1 0 011-1h12a1 1 0 110 2H4a1 1 0 01-1-1zM3 10a1 1 0 011-1h12a1 1 0 110 2H4a1 1 0 01-1-1zM3 15a1 1 0 011-1h12a1 1 0 110 2H4a1 1 0 01-1-1z"
                      clip-rule="evenodd"
                    ></path>
                  </svg>
                  <svg
                    class="hidden w-6 h-6"
                    fill="currentColor"
                    viewBox="0 0 20 20"
                    xmlns="http://www.w3.org/2000/svg"
                  >
                    <path
                      fill-rule="evenodd"
                      d="M4.293 4.293a1 1 0 011.414 0L10 8.586l4.293-4.293a1 1 0 111.414 1.414L11.414 10l4.293 4.293a1 1 0 01-1.414 1.414L10 11.414l-4.293 4.293a1 1 0 01-1.414-1.414L8.586 10 4.293 5.707a1 1 0 010-1.414z"
                      clip-rule="evenodd"
                    ></path>
                  </svg>
                </button>
              </div>

              <div class="lg:hidden ">
                <div :class="modal ? 'absolute left-0 top-0 bg-white z-50 sm:w-[50%] w-[80%] h-[100vh] ' : 'hidden '">
                  <button @click="toggleModal" class="absolute text-[30px] right-2 top-2 text-white"><i class='bx bx-x' ></i></button>
                  <div class="pl-5 py-5 bg-[#EFF2F4]">
                    <img src="../store/img/img/Avatar-2.png" alt=""  class=""/>
                    <h1 class="font-normal mt-3"> <a href="#">Sign in</a> | <a href="#">Register</a></h1>
                  </div>
                  <ul>
                    <li class="pl-5 py-3.5 flex items-center gap-4">
                      <i class='bx bx-home text-[25px] text-[#8B96A5]' ></i>
                      <a href="#" class="font-normal">Home</a>
                    </li>
                    <li class="pl-5 py-3.5 flex items-center gap-4">
                      <i class='bx bx-list-ul text-[25px] text-[#8B96A5]'></i>
                      <a href="#" class="font-normal">Categories</a>
                    </li>
                    <li class="pl-5 py-3.5 flex items-center gap-4">
                      <i class='bx bx-heart text-[25px] text-[#8B96A5]' ></i>
                      <a href="#" class="font-normal">Favorites</a>
                    </li>
                    <li class="pl-5 py-3.5 flex items-center gap-4 border-b">
                      <i class='bx bx-box text-[25px] text-[#8B96A5]' ></i>
                      <a href="#" class="font-normal">My orders</a>
                    </li>
                    <li class="pl-5 py-3.5 flex items-center gap-4">
                      <i class='bx bx-globe text-[25px] text-[#8B96A5]' ></i>
                      <a href="#" class="font-normal">English | USD</a>
                    </li>
                    <li class="pl-5 py-3.5 flex items-center gap-4">
                      <i class='bx bx-headphone text-[25px] text-[#8B96A5]' ></i>
                      <a href="#" class="font-normal">Contact us</a>
                    </li>
                    <li class="pl-5 py-3.5 flex items-center gap-4 border-b">
                      <i class='bx bxs-business text-[25px] text-[#8B96A5]' ></i>
                      <a href="#" class="font-normal">About</a>
                    </li>
                    <li class="pl-16 py-3.5 flex items-center gap-4">
                      <a href="#" class="font-normal">User agreement</a>
                    </li>
                    <li class="pl-16 py-3.5 flex items-center gap-4">
                      <a href="#" class="font-normal">Partnership</a>
                    </li>
                    <li class="pl-16 py-3.5 flex items-center gap-4">
                      <a href="#" class="font-normal">Privacy policy</a>
                    </li>
                  </ul>
                </div>
              </div>

              <a href="/" class="flex items-center">
                <img
                  src="../public/favicon.png"
                  class="mr-3 h-6 sm:h-9"
                  alt="Flowbite Logo"
                />
                <span
                  class="self-center text-xl font-semibold whitespace-nowrap text-[#8CB7F5]"
                  >Brand</span
                >
              </a>
            </div>

            <div class="flex item-center justify-between gap-3 lg:hidden">
              <a href="#">
                <img src="../store/img/icon/shopping_cart.svg" alt="" />
              </a>
              <a href="#">
                <img src="../store/img/icon/person.svg" alt="" />
              </a>
            </div>

            <form class="w-full lg:w-[50%] mt-3 lg:mt-0">
              <div
                class="flex border-2 border-gray-300 lg:border-[rgba(18,127,255,1)] rounded-[12px] w-full"
              >
                <div class="relative w-full flex items-center">
                  <i class="bx bx-search ml-5 text-[20px] text-gray-400 lg:hidden"></i>
                  <input
                    type="search"
                    id="search-dropdown"
                    class="block py-2.5 pl-2 xl:p-2.5 w-full z-20 text-sm text-gray-900 md:rounded-l-[12px] rounded-[15px] lg:bg-[#F7FAFC] xl:bg-gray-50 outline-none"
                    placeholder="Search..."
                    required
                  />
                  <button
                    @click="toggleAll"
                    id="dropdown-button"
                    data-dropdown-toggle="dropdown"
                    class="hidden lg:flex flex-shrink-0 z-10 inline-flex items-center py-2.5 px-4 text-sm font-medium text-center text-gray-900 border-l border-blue-500"
                    type="button"
                  >
                    All categories
                    <svg
                      aria-hidden="true"
                      class="w-4 h-4 ml-1"
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
                  <div
                    id="dropdown"
                    :class="
                      all
                        ? 'absolute z-50 right-20 top-12  bg-gray-200 rounded-lg shadow w-44'
                        : 'hidden'
                    "
                  >
                    <ul
                      class="py-2 text-sm text-gray-700"
                      aria-labelledby="dropdown-button"
                    >
                      <li>
                        <button type="button" class="inline-flex w-full px-4 py-2">
                          Mockups
                        </button>
                      </li>
                      <li>
                        <button type="button" class="inline-flex w-full px-4 py-2">
                          Templates
                        </button>
                      </li>
                      <li>
                        <button type="button" class="inline-flex w-full px-4 py-2">
                          Design
                        </button>
                      </li>
                      <li>
                        <button type="button" class="inline-flex w-full px-4 py-2">
                          Logos
                        </button>
                      </li>
                    </ul>
                  </div>
                  <button
                    type="submit"
                    class="hidden lg:block p-2.5 text-sm font-medium text-white bg-[rgba(18,127,255,1)] rounded-r-lg hover:bg-blue-800 w-[150px]"
                  >
                    <span class="">Search</span>
                  </button>
                </div>
              </div>
            </form>

            <div
              class="hidden justify-between items-center w-full lg:flex lg:w-auto lg:order-1"
              id="mobile-menu-2"
            >
              <ul class="flex items-center gap-5">
                <li
                  class="flex flex-col justify-center items-center text-[#8B96A5] hover:text-blue-500"
                >
                  <i class="bx bxs-user text-[25px]"></i>
                  <a href="#" class="block" aria-current="page">Profile</a>
                </li>
                <li
                  class="flex flex-col justify-center items-center text-[#8B96A5] hover:text-blue-500"
                >
                  <i class="bx bxs-message-detail text-[25px]"></i>
                  <a href="#" class="block">Message</a>
                </li>
                <li
                  class="flex flex-col justify-center items-center text-[#8B96A5] hover:text-blue-500"
                >
                  <i class="bx bxs-heart text-[25px]"></i>
                  <a href="#" class="block">Orders</a>
                </li>
                <NuxtLink
                  to="/cart"
                  class="flex flex-col justify-center items-center text-[#8B96A5] hover:text-blue-500"
                >
                  <i class="bx bxs-cart text-[25px]"></i>
                  <a class="block">My cart</a>
                </NuxtLink>
              </ul>
            </div>
          </div>
        </nav>
      </div>
    </div>
    <div class="hidden bg-white border-gray-200 border-b lg:block">
      <div class="container mx-auto px-5">
        <nav class="py-3">
          <div class="flex flex-wrap justify-between items-center">
            <div class="w-full md:block md:w-auto" id="navbar-dropdown">
              <ul class="flex items-center gap-6">
                <li class="flex items-center gap-2 hover:text-blue-500">
                  <i class="bx bx-menu text-[25px]"></i>
                  <a href="#" class="block" aria-current="page">All category</a>
                </li>
                <li>
                  <a href="#" class="block hover:text-blue-500" aria-current="page"
                    >Hot offers</a
                  >
                </li>
                <li>
                  <a href="#" class="block hover:text-blue-500">Gift boxes</a>
                </li>
                <li>
                  <a href="#" class="block hover:text-blue-500">Projects</a>
                </li>
                <li>
                  <a href="#" class="block hover:text-blue-500">Menu item</a>
                </li>
                <li>
                  <button
                    @click="toggleMenu"
                    id="dropdownNavbarLink"
                    data-dropdown-toggle="dropdownNavbar"
                    class="flex items-center justify-between w-full rounded hover:text-blue-500"
                  >
                    Help
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
                      menu ? 'z-10 absolute font-normal bg-gray-200 rounded' : 'hidden'
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
                </li>
              </ul>
            </div>

            <div class="flex items-center">
              <ul class="flex items-center gap-5">
                <li>
                  <button
                    @click="toggleEnglish"
                    id="dropdownNavbarLink"
                    data-dropdown-toggle="dropdownNavbar"
                    class="flex items-center justify-between w-full rounded hover:text-blue-500"
                  >
                    English, USD
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
                      english ? 'z-10 absolute font-normal bg-gray-200 rounded' : 'hidden'
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
                </li>
                <li>
                  <button
                    @click="toggleShip"
                    id="dropdownNavbarLink"
                    data-dropdown-toggle="dropdownNavbar"
                    class="flex items-center justify-between gap-1 w-full rounded hover:text-blue-500"
                  >
                    Ship to
                    <img src="../store/img/flag/DE@2x.png" alt="" />
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
                      ship ? 'z-10 absolute font-normal bg-gray-200 rounded' : 'hidden'
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
                </li>
              </ul>
            </div>
          </div>
        </nav>
      </div>
    </div>
  </header>
</template>

<script setup>
import { ref } from "vue";

const all = ref(false);
const toggleAll = () => (all.value = !all.value);

const menu = ref(false);
const toggleMenu = () => (menu.value = !menu.value);

const modal = ref(false);
const toggleModal = () => (modal.value = !modal.value);

const english = ref(false);
const toggleEnglish = () => (english.value = !english.value);

const ship = ref(false);
const toggleShip = () => (ship.value = !ship.value);
</script>

<style lang="scss" scoped>
.router-link-exact-active {
  font-weight: 800;
  color: rgb(59, 59, 250);
  border-bottom: 1px solid rgb(5, 5, 244);
}
</style>
