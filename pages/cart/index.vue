<template>
  <div class="container mx-auto px-5 mt-36">
    <h1 class="text-[24px] font-semibold mb-5">My cart (3)</h1>
    <div class="w-full flex gap-5 mb-5">
      <div class="border rounded-lg bg-white p-5 w-[75%]">
        <div class="border-b flex justify-between">
          <div class="flex gap-4">
            <div
              class="rounded-lg bg-[rgba(224,224,224,1)] h-[100px] w-[100px] flex items-center justify-center"
            >
              <img
                src="../../store/img/rec-items/finka.png"
                alt=""
                class="w-[52.58px] h-[59.73px]"
              />
            </div>
            <div>
              <h2 class="font-medium mb-3">
                T-shirts with multiple colors, for men and lady
              </h2>
              <p class="text-[#8B96A5] font-normal mb-5">
                Size: medium, Color: blue, Material: Plastic <br />
                Seller: Artel Market
              </p>
              <div class="flex items-center gap-2 mb-5">
                <button
                  class="text-[#FA3434] text-[13px] py-2 px-4 rounded-lg bg-white font-medium border hover:border-[#FA3434]"
                >
                  Remove
                </button>
                <button
                  class="text-[#0D6EFD] text-[13px] py-2 px-4 rounded-lg bg-white font-medium border hover:border-[#0D6EFD]"
                >
                  Save for later
                </button>
              </div>
            </div>
          </div>
          <div class="flex flex-col items-end gap-3 mt-3">
            <h2 class="font-medium">$78.99</h2>
            <div>
              <button
                @click="toggleMenu"
                id="dropdownNavbarLink"
                data-dropdown-toggle="dropdownNavbar"
                class="flex items-center justify-between w-full rounded-lg gap-10 px-4 py-2 border"
              >
                Qty: 9
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
                :class="menu ? 'z-10 absolute font-normal bg-gray-200 rounded' : 'hidden'"
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
          </div>
        </div>

        <div class="border-b mt-5 flex justify-between">
          <div class="flex gap-4">
            <div
              class="rounded-lg bg-[rgba(224,224,224,1)] h-[100px] w-[100px] flex items-center justify-center"
            >
              <img
                src="../../store/img/rec-items/finka.png"
                alt=""
                class="w-[52.58px] h-[59.73px]"
              />
            </div>
            <div>
              <h2 class="font-medium mb-3">
                T-shirts with multiple colors, for men and lady
              </h2>
              <p class="text-[#8B96A5] font-normal mb-5">
                Size: medium, Color: blue, Material: Plastic <br />
                Seller: Artel Market
              </p>
              <div class="flex items-center gap-2 mb-5">
                <button
                  class="text-[#FA3434] text-[13px] py-2 px-4 rounded-lg bg-white font-medium border hover:border-[#FA3434]"
                >
                  Remove
                </button>
                <button
                  class="text-[#0D6EFD] text-[13px] py-2 px-4 rounded-lg bg-white font-medium border hover:border-[#0D6EFD]"
                >
                  Save for later
                </button>
              </div>
            </div>
          </div>
          <div class="flex flex-col items-end gap-3 mt-3">
            <h2 class="font-medium">$39.00</h2>
            <div>
              <button
                @click="toggleMenu"
                id="dropdownNavbarLink"
                data-dropdown-toggle="dropdownNavbar"
                class="flex items-center justify-between w-full rounded-lg gap-10 px-4 py-2 border"
              >
                Qty: 9
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
                :class="menu ? 'z-10 absolute font-normal bg-gray-200 rounded' : 'hidden'"
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
          </div>
        </div>

        <div class="border-b mt-5 flex justify-between">
          <div class="flex gap-4">
            <div
              class="rounded-lg bg-[rgba(224,224,224,1)] h-[100px] w-[100px] flex items-center justify-center"
            >
              <img
                src="../../store/img/rec-items/finka.png"
                alt=""
                class="w-[52.58px] h-[59.73px]"
              />
            </div>
            <div>
              <h2 class="font-medium mb-3">
                T-shirts with multiple colors, for men and lady
              </h2>
              <p class="text-[#8B96A5] font-normal mb-5">
                Size: medium, Color: blue, Material: Plastic <br />
                Seller: Artel Market
              </p>
              <div class="flex items-center gap-2 mb-5">
                <button
                  class="text-[#FA3434] text-[13px] py-2 px-4 rounded-lg bg-white font-medium border hover:border-[#FA3434]"
                >
                  Remove
                </button>
                <button
                  class="text-[#0D6EFD] text-[13px] py-2 px-4 rounded-lg bg-white font-medium border hover:border-[#0D6EFD]"
                >
                  Save for later
                </button>
              </div>
            </div>
          </div>
          <div class="flex flex-col items-end gap-3 mt-3">
            <h2 class="font-medium">$170.50</h2>
            <div>
              <button
                @click="toggleMenu"
                id="dropdownNavbarLink"
                data-dropdown-toggle="dropdownNavbar"
                class="flex items-center justify-between w-full rounded-lg gap-10 px-4 py-2 border"
              >
                Qty: 9
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
                :class="menu ? 'z-10 absolute font-normal bg-gray-200 rounded' : 'hidden'"
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
          </div>
        </div>

        <div class="flex items-center justify-between mt-5">
          <button
            class="bg-[rgba(18,127,255,1)] text-white flex items-center gap-3 py-2 px-4 rounded-lg"
          >
            <i class="bx bx-left-arrow-alt text-[30px]"></i>Back to shop
          </button>
          <button
            class="bg-white border text-[#0D6EFD] rounded-lg px-4 py-2 hover:border-[#0D6EFD]"
          >
            Remove all
          </button>
        </div>
      </div>

      <div class="w-[25%]">
        <div class="border rounded-lg p-5 bg-white mb-5">
          <p class="text-[#505050] font-normal mb-5">Have a coupon?</p>
          <div class="flex border rounded-lg w-full">
            <input
              type="text"
              placeholder="Add coupon"
              class="p-2 outline-none rounded-l-lg w-[70%]"
            />
            <button class="p-2 rounded-r-lg border-l text-[#0D6EFD] font-medium w-[30%]">
              Apply
            </button>
          </div>
        </div>

        <div class="border rounded-lg p-5 bg-white shadow-lg">
          <div class="flex items-center justify-between border-b pb-5">
            <div class="flex flex-col gap-1">
              <p class="text-[#505050] font-normal">Subtotal:</p>
              <p class="text-[#505050] font-normal">Discount:</p>
              <p class="text-[#505050] font-normal">Tax:</p>
            </div>
            <div class="flex flex-col gap-1">
              <p class="text-[#505050] font-normal">$1403.97</p>
              <p class="text-[#FA3434] font-normal">- $60.00</p>
              <p class="text-[#00B517] font-normal">+ $14.00</p>
            </div>
          </div>

          <div class="py-5">
            <div class="flex items-center justify-between mb-5">
              <p class="font-semibold">Total:</p>
              <p class="font-semibold text-[20px]">$1357.97</p>
            </div>
            <button
              class="text-white text-[18px] font-medium bg-[#00B517] border border-[#00B517] rounded-lg py-5 w-full hover:bg-white hover:text-[#00B517] mb-5"
            >
              Checkout
            </button>
            <div class="flex items-center gap-3 justify-center">
              <img src="../../store/img/payment/payment-1.png" alt="" />
              <img src="../../store/img/payment/payment-2.png" alt="" />
              <img src="../../store/img/payment/payment-3.png" alt="" />
              <img src="../../store/img/payment/payment-4.png" alt="" />
              <img src="../../store/img/payment/payment-5.png" alt="" />
            </div>
          </div>
        </div>
      </div>
    </div>

    <div class="w-[75%] flex items-center gap-10 mb-8">
      <div class="w-[28%] flex items-center gap-3">
        <i class='bx bxs-lock-alt bg-[#DEE2E7] p-4 rounded-full text-[25px] text-[#8B96A5]'></i>
        <div >
          <p class="font-normal">Secure payment</p>
          <p class="text-[#A9ACB0] font-normal">Have you ever finally just </p>
        </div>
      </div>

      <div class="w-[28%] flex items-center gap-3">
        <i class='bx bxs-message-detail bg-[#DEE2E7] p-4 rounded-full text-[25px] text-[#8B96A5]'></i>
        <div>
          <p class="font-normal">Customer support</p>
          <p class="text-[#A9ACB0] font-normal">Have you ever finally just </p>
        </div>
      </div>

      <div class="w-[28%] flex items-center gap-3">
        <i class='bx bxs-truck bg-[#DEE2E7] p-4 rounded-full text-[25px] text-[#8B96A5]'></i>
        <div>
          <p class="font-normal">Free delivery</p>
          <p class="text-[#A9ACB0] font-normal">Have you ever finally just</p>
        </div>
      </div>
    </div>

    <div class="w-full p-5 border rounded-lg bg-white mb-5">
      <h2 class="text-[20px] font-semibold mb-5">Saved for later</h2>
        <div class="flex gap-5">
          <div v-for="cart in cartLink" :key="cart.id" class="w-[25%]">
          <div class="flex items-center justify-center py-12 bg-[#EEEEEE] rounded-lg mb-2 ">
            <img :src="cart.img" alt="" class="w-[194px] h-[200px] bg-transparent">
          </div>
          <div>
            <h3 class="text-[18px] font-semibold mb-3">{{ cart.price }}</h3>
            <p class="text-[#606060] font-normal w-[215.8px] mb-4">{{ cart.name }}</p>
            <button class="text-[#0D6EFD] flex items-center gap-3 border p-2 rounded-lg hover:border-[#0D6EFD]"> <i class='bx bx-cart text-[25px]'></i>Move to cart</button>
          </div>
        </div>
        </div>
    </div>
  </div>
</template>

<script setup>
import {ref} from "vue"
import { cartLinks } from "~/store/info/cart";

const cartLink = ref(cartLinks);
</script>

<style lang="scss" scoped></style>
