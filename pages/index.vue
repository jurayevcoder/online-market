<template>
  <div class="container mx-auto p-5">
    <div
      class="hidden mt-32 lg:flex items-center justify-between gap-5 border border-[#DEE2E7] rounded-lg p-5 mb-5 bg-white"
    >
      <div class="flex flex-col items-start w-[30%]">
        <button
          class="text-left text-[#1C1C1C] bg-white hover:bg-[#E5F1FF] p-[10.80px] rounded-lg w-full"
        >
          Automobiles
        </button>
        <button
          class="text-left text-[#1C1C1C] bg-white hover:bg-[#E5F1FF] p-[10.80px] rounded-lg w-full"
        >
          Clothes and wear
        </button>
        <button
          class="text-left text-[#1C1C1C] bg-white hover:bg-[#E5F1FF] p-[10.80px] rounded-lg w-full"
        >
          Home interiors
        </button>
        <button
          class="text-left text-[#1C1C1C] bg-white hover:bg-[#E5F1FF] p-[10.80px] rounded-lg w-full"
        >
          Computer and tech
        </button>
        <button
          class="text-left text-[#1C1C1C] bg-white hover:bg-[#E5F1FF] p-[10.80px] rounded-lg w-full"
        >
          Tools, equipments
        </button>
        <button
          class="text-left text-[#1C1C1C] bg-white hover:bg-[#E5F1FF] p-[10.80px] rounded-lg w-full"
        >
          Sports and outdoor
        </button>
        <button
          class="text-left text-[#1C1C1C] bg-white hover:bg-[#E5F1FF] p-[10.80px] rounded-lg w-full"
        >
          Animal and pets
        </button>
        <button
          class="text-left text-[#1C1C1C] bg-white hover:bg-[#E5F1FF] p-[10.80px] rounded-lg w-full"
        >
          Machinery tools
        </button>
        <button
          class="text-left text-[#1C1C1C] bg-white hover:bg-[#E5F1FF] p-[10.80px] rounded-lg w-full"
        >
          More category
        </button>
      </div>

      <div
        class="w-[85%] h-[410px] pt-20 pl-12 bg-no-repeat bg-cover bg-center bg-[url('/store/img/img/Banner.jpg')]"
      >
        <p class="text-[24px] text-[#1C1C1C]">Latest trending</p>
        <h1 class="text-[32px] text-[#1C1C1C] font-bold mb-5">Electronic items</h1>
        <button
          class="bg-white px-3 py-1.5 rounded-lg hover:bg-blue-500 hover:text-white"
        >
          Learn more
        </button>
      </div>

      <div class="w-[25%]">
        <div class="bg-[#E3F0FF] w-full p-4 rounded-lg mb-4">
          <div class="flex items-center gap-3 mb-4">
            <img
              src="../store/img/img/Avatar.png"
              alt=""
              class="rounded-full w-[44px] h-[44px]"
            />
            <div class="text-[#1C1C1C]">
              <p>Hi, user</p>
              <p>let's get stated</p>
            </div>
          </div>
          <button
            class="bg-[rgba(18,127,255,1)] text-white rounded-lg w-full py-1 mb-2 hover:text-[rgba(18,127,255,1)] hover:bg-[#E3F0FF] border hover:border-[rgba(18,127,255,1)]"
          >
            Join now
          </button>
          <button
            class="bg-white text-[rgba(18,127,255,1)] rounded-lg w-full py-1 border hover:border-[rgba(18,127,255,1)] hover:bg-[#E3F0FF]"
          >
            Log in
          </button>
        </div>
        <div class="bg-[#F38332] w-full p-4 rounded-lg text-white mb-4">
          <p>
            Get US $10 off <br />
            with a new <br />
            supplier
          </p>
        </div>
        <div class="bg-[#55BDC4] w-full p-4 rounded-lg text-white">
          <p>
            Send quotes with <br />
            supplier <br />
            preferences
          </p>
        </div>
      </div>
    </div>

    <div class="hidden lg:flex border border-[#DEE2E7] rounded-lg mb-5 bg-white">
      <div class="px-5 py-6 w-[23%] border-r">
        <h1 class="text-[20px] text-[#1C1C1C] font-bold">Deals and offers</h1>
        <p class="text-[#8B96A5]">Hygiene equipments</p>
        <div class="flex items-center gap-3 mt-4">
          <div class="text-center text-white bg-[#606060] rounded-lg px-2 py-1">
            <p class="font-bold">04</p>
            <p>Days</p>
          </div>
          <div class="text-center text-white bg-[#606060] rounded-lg px-2 py-1">
            <p class="font-bold">13</p>
            <p>Hour</p>
          </div>
          <div class="text-center text-white bg-[#606060] rounded-lg px-3 py-1">
            <p class="font-bold">34</p>
            <p>Min</p>
          </div>
          <div class="text-center text-white bg-[#606060] rounded-lg px-3 py-1">
            <p class="font-bold">56</p>
            <p>Sec</p>
          </div>
        </div>
      </div>
      <div class="flex w-[77%]">
        <div
          v-for="link in offerLink"
          :key="link.id"
          :class="
            link.id !== offerLink.length
              ? 'flex flex-col justify-center items-center border-r py-6 px- w-[20%]'
              : 'flex flex-col justify-center items-center py-6 px- w-[20%]'
          "
        >
          <div class="h-[120px]">
            <img :src="link.img" alt="" class="" />
          </div>
          <div class="flex flex-col items-center gap-2 mt-5">
            <a
              href="#"
              class="text-[#1C1C1C] hover:underline hover:text-[rgba(18,127,255,1)]"
              >{{ link.name }}</a
            >
            <p
              class="text-[#EB001B] text-[14px] rounded-full py-1 px-4 flex justify-center bg-[#FFE3E3]"
            >
              {{ link.chegirma }}
            </p>
          </div>
        </div>
      </div>
    </div>

    <div class="hidden lg:flex border border-[#DEE2E7] rounded-lg w-[100%] mb-5 bg-white">
      <div
        class="w-[23%] pt-5 pl-5 bg-no-repeat bg-cover bg-center bg-[url('/store/img/img/image92.png')]"
      >
        <p class="text-[20px] font-bold mb-5">
          Home and <br />
          outdoor
        </p>
        <button class="bg-white py-2 px-5 rounded-lg hover:bg-gray-300 hover:text-white">
          Source now
        </button>
      </div>

      <div class="flex flex-col w-[77%]">
        <div class="flex border-b">
          <div
            v-for="home in homeLink_1"
            :key="home.id"
            :class="
              home.id !== homeLink_1.length
                ? 'flex flex-col border-r w-[25%] py-4 px-6'
                : 'flex flex-col w-[25%] py-4 px-6'
            "
          >
            <a href="#" class="hover:underline hover:text-[rgba(18,127,255,1)]">{{
              home.name
            }}</a>
            <div class="flex items-center justify-between">
              <p class="text-[#8B96A5] text-[13px]">
                From <br />
                {{ home.price }}
              </p>
              <img :src="home.img" alt="" />
            </div>
          </div>
        </div>

        <div class="flex">
          <div
            v-for="hom in homeLink_2"
            :key="hom.id"
            :class="
              hom.id !== homeLink_2.length
                ? 'flex flex-col border-r w-[25%] py-4 px-6'
                : 'flex flex-col w-[25%] py-4 px-6'
            "
          >
            <a href="#" class="hover:underline hover:text-[rgba(18,127,255,1)]">{{
              hom.name
            }}</a>
            <div class="flex items-center justify-between">
              <p class="text-[#8B96A5] text-[13px]">
                From <br />
                {{ hom.price }}
              </p>
              <img :src="hom.img" alt="" />
            </div>
          </div>
        </div>
      </div>
    </div>

    <div class="hidden lg:flex border border-[#DEE2E7] rounded-lg w-[100%] mb-5 bg-white">
      <div
        class="w-[23%] pt-5 pl-5 bg-no-repeat bg-cover bg-center bg-[url('/store/img/img/image98.png')]"
      >
        <p class="text-[20px] font-bold mb-5">
          Consumer <br />
          electronics and <br />
          gadgets
        </p>
        <button class="bg-white py-2 px-5 rounded-lg hover:bg-gray-300 hover:text-white">
          Source now
        </button>
      </div>

      <div class="flex flex-col w-[77%]">
        <div class="flex border-b">
          <div
            v-for="elec in elecLink_1"
            :key="elec.id"
            :class="
              elec.id !== elecLink_1.length
                ? 'flex flex-col border-r w-[25%] py-4 px-6'
                : 'flex flex-col w-[25%] py-4 px-6'
            "
          >
            <a href="#" class="hover:underline hover:text-[rgba(18,127,255,1)]">{{
              elec.name
            }}</a>
            <div class="flex items-center justify-between">
              <p class="text-[#8B96A5] text-[13px]">
                From <br />
                {{ elec.price }}
              </p>
              <img :src="elec.img" alt="" />
            </div>
          </div>
        </div>

        <div class="flex">
          <div
            v-for="elek in elecLink_2"
            :key="elek.id"
            :class="
              elek.id !== elecLink_2.length
                ? 'flex flex-col border-r w-[25%] py-4 px-6'
                : 'flex flex-col w-[25%] py-4 px-6'
            "
          >
            <a href="#" class="hover:underline hover:text-[rgba(18,127,255,1)]">{{
              elek.name
            }}</a>
            <div class="flex items-center justify-between">
              <p class="text-[#8B96A5] text-[13px]">
                From <br />
                {{ elek.price }}
              </p>
              <img :src="elek.img" alt="" />
            </div>
          </div>
        </div>
      </div>
    </div>

    <div
      class="hidden lg:flex rounded-lg w-[100%] bg-no-repeat bg-cover bg-center bg-[url('/store/img/img/Group982.png')] p-10 justify-between mb-5"
    >
      <div>
        <h3 class="text-[32px] text-white font-bold mb-5">
          An easy way to send <br />
          requests to all suppliers
        </h3>
        <p class="text-white">
          Lorem ipsum dolor sit amet, consectetur adipisicing <br />
          elit, sed do eiusmod tempor incididunt.
        </p>
      </div>

      <div class="bg-white rounded-lg w-[500px] p-5">
        <h3 class="text-[20px] font-normal mb-5">Send quote to suppliers</h3>
        <input
          type="text"
          placeholder="What item you need?"
          class="outline-none border rounded-lg w-full p-2 mb-3 placeholder-black"
        />
        <textarea
          name=""
          id=""
          cols="30"
          rows="10"
          placeholder="Type more details"
          class="outline-none border p-2 rounded-lg w-full h-[73px] mb-2"
        ></textarea>
        <div class="relative flex items-center mb-5 gap-3">
          <input
            type="text"
            placeholder="Quantity"
            class="outline-none border rounded-lg p-2 placeholder-black"
          />
          <button
            @click="toggleModal"
            id="dropdownNavbarLink"
            data-dropdown-toggle="dropdownNavbar"
            class="flex items-center justify-between w-[100px] rounded border p-2"
          >
            Pcs
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
              modal
                ? 'z-50 absolute font-normal bg-white rounded right-20 top-12 w-[100px]'
                : 'hidden'
            "
          >
            <ul class="py-2 text-sm text-gray-900" aria-labelledby="dropdownLargeButton">
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
        <button
          class="bg-[rgba(18,127,255,1)] text-white rounded-lg border border-[rgba(18,127,255,1)] px-4 py-2 hover:bg-white hover:text-[rgba(18,127,255,1)]"
        >
          Send inquiry
        </button>
      </div>
    </div>

    <div class="hidden lg:block w-[100%]">
      <h1 class="text-[24px] font-semibold mb-5">Recommended items</h1>
      <div class="w-[100%] flex flex-wrap gap-[1.5%]">
        <div
          v-for="item in recItemsLink"
          :key="item.id"
          class="border w-[18.8%] p-5 rounded-lg flex flex-col items-center mb-5 bg-white cursor-pointer"
        >
          <img :src="item.img" alt="" class="w-[150.22px] h-[170.67px] mb-[20px]" />
          <div class="">
            <h2 class="font-medium mb-[5px]">{{ item.price }}</h2>
            <p class="text-[#8B96A5] font-normal w-[186px]">{{ item.info }}</p>
          </div>
        </div>
      </div>
    </div>

    <div class="hidden lg:block w-[100%] mb-5">
      <h1 class="text-[24px] font-semibold mb-5">Our extra services</h1>
      <div class="w-[100%] flex gap-5">
        <div
          v-for="ser in serviceLink"
          :key="ser.id"
          class="w-[25%] border rounded-lg relative bg-white"
        >
          <img :src="ser.img" alt="" class="w-full rounded-t-lg bg-[rgba(0,0,0,0.9)]" />
          <p class="font-medium my-5 ml-5 w-[168px]">
            {{ ser.name }}
          </p>
          <button
            class="absolute right-8 top-[100px] bg-[#D1E7FF] p-5 flex items-center justify-center rounded-full text-[25px] border-2 border-white"
          >
            <i :class="ser.icon"></i>
          </button>
        </div>
      </div>
    </div>

    <div class="hidden lg:block w-[100%]">
      <h1 class="text-[24px] font-semibold mb-5">Suppliers by region</h1>
      <div class="w-[100%] flex flex-wrap gap-4">
        <div
          v-for="flag in flagLink"
          :key="flag.id"
          class="w-[18.9%] flex items-center gap-3"
        >
          <img :src="flag.img" alt="" class="w-[28px] h-[20px]" />
          <div>
            <h2 class="font-normal">{{ flag.name }}</h2>
            <p class="text-[13px] text-[#8B96A5] font-normal">{{ flag.info }}</p>
          </div>
        </div>
      </div>
    </div>
  </div>

  <!-- Response -->

  <div class="lg:hidden sm:mt-[105px] mt-20 mb-5">
    <div class="container mx-auto px-5">
      <div class="flex flex-wrap items-center gap-3 w-full">
        <button class="text-[#0D6EFD] font-normal bg-[#EFF2F4] py-1.5 px-2 rounded-lg">
          All category
        </button>
        <button class="text-[#0D6EFD] font-normal bg-[#EFF2F4] py-1.5 px-2 rounded-lg">
          Gadgets
        </button>
        <button class="text-[#0D6EFD] font-normal bg-[#EFF2F4] py-1.5 px-2 rounded-lg">
          Clocthes
        </button>
        <button class="text-[#0D6EFD] font-normal bg-[#EFF2F4] py-1.5 px-2 rounded-lg">
          Accessory
        </button>
        <button class="text-[#0D6EFD] font-normal bg-[#EFF2F4] py-1.5 px-2 rounded-lg">
          Tablets
        </button>
        <button class="text-[#0D6EFD] font-normal bg-[#EFF2F4] py-1.5 px-2 rounded-lg">
          Phones
        </button>
        <button class="text-[#0D6EFD] font-normal bg-[#EFF2F4] py-1.5 px-2 rounded-lg">
          Phones
        </button>
      </div>
    </div>
  </div>

  <div
    class="lg:hidden bg-no-repet bg-cover bg-center bg-[url('/store/img/img/Banner.jpg')] sm:py-20 py-5 sm:h-[400px] mb-5"
  >
    <div class="container mx-auto px-5">
      <h1 class="font-normal sm:text-[32px] text-[18px]">Latest trending</h1>
      <h2 class="text-[18px] sm:text-[32px] font-semibold mb-5">Electronic items</h2>
      <button
        class="text-[13px] text-[#0D6EFD] font-medium bg-white rounded-lg py-2 px-4 mb-12"
      >
        Learn more
      </button>
    </div>
  </div>

  <div class="lg:hidden container mx-auto px-5 flex items-center justify-between mb-5">
    <div class="">
      <h2 class="text-[18px] font-semibold">Deals and offers</h2>
      <p class="text-[13px] font-normal tex-[#505050]">Electronic equipments</p>
    </div>
    <div class="flex items-center gap-2">
      <div class="flex flex-col items-center bg-[#EFF2F4] px-3 py-1">
        <h3 class="text-[#8B96A5] font-semibold">13</h3>
        <p class="text-[13px] text-[#8B96A5] font-normal">Hour</p>
      </div>
      <div class="flex flex-col items-center bg-[#EFF2F4] px-3 py-1">
        <h3 class="text-[#8B96A5] font-semibold">34</h3>
        <p class="text-[13px] text-[#8B96A5] font-normal">Min</p>
      </div>
      <div class="flex flex-col items-center bg-[#EFF2F4] px-3 py-1">
        <h3 class="text-[#8B96A5] font-semibold">56</h3>
        <p class="text-[13px] text-[#8B96A5] font-normal">Sec</p>
      </div>
    </div>
  </div>

  <div class="lg:hidden container mx-auto px-5 flex mb-5 items-center justify-between border py-5">
    <button
      @click="back"
      :class="0 == sch ? 'text-gray-200 text-[50px]' : 'text-gray-400 text-[50px]'"
    >
      <i class="bx bxs-chevron-left-circle"></i>
    </button>
    <div class="w-full flex items-center justify-center">
      <div class="flex items-center w-[80%] gap-5">
        <div
          class="flex flex-col justify-center items-center border rounded-lg py-6 w-full"
        >
          <div class="h-[120px]">
            <img :src="offerLink[sch].img" alt="" />
          </div>
          <div class="flex flex-col items-center gap-2 mt-5">
            <a
              href="#"
              class="text-[#1C1C1C] hover:underline hover:text-[rgba(18,127,255,1)]"
              >{{ offerLink[sch].name }}</a
            >
            <p
              class="text-[#EB001B] text-[14px] rounded-full py-1 px-4 flex justify-center bg-[#FFE3E3]"
            >
              {{ offerLink[sch].chegirma }}
            </p>
          </div>
        </div>

        <div
          class="hidden sm:flex flex-col justify-center items-center border rounded-lg py-6 w-full"
        >
          <div class="h-[120px]">
            <img :src="offerLink[sch + 1].img" alt="" class="" />
          </div>
          <div class="flex flex-col items-center gap-2 mt-5">
            <a
              href="#"
              class="text-[#1C1C1C] hover:underline hover:text-[rgba(18,127,255,1)]"
              >{{ offerLink[sch + 1].name }}</a
            >
            <p
              class="text-[#EB001B] text-[14px] rounded-full py-1 px-4 flex justify-center bg-[#FFE3E3]"
            >
              {{ offerLink[sch + 1].chegirma }}
            </p>
          </div>
        </div>
      </div>
    </div>
    <button
      @click="next"
      :class="
        offerLink.length - 2 == sch
          ? 'text-gray-200 text-[50px]'
          : 'text-gray-400 text-[50px]'
      "
    >
      <i class="bx bxs-chevron-right-circle"></i>
    </button>
  </div>

  <div class="lg:hidden">
   <div class="container mx-auto px-5 mb-5">
    <h1 class="text-[18px] font-semibold">Home and outdoor</h1>
   </div>
    <div class="container mx-auto px-5 flex mb-5 items-center justify-between border py-5">
      <button
        @click="backHome"
        :class="0 == id ? 'text-gray-200 text-[50px]' : 'text-gray-400 text-[50px]'"
      >
        <i class="bx bxs-chevron-left-circle"></i>
      </button>

      <div class="w-full flex items-center justify-center">
        <div class="flex items-center w-[80%] gap-5">
          <div
            class="flex flex-col justify-center items-center border rounded-lg py-6 w-full"
          >
            <div class="h-[120px]">
              <img :src="homeLink[id].img" alt="" class="w-28 h-28"/>
            </div>
            <div class="flex flex-col items-center gap-2 mt-5">
              <a
                href="#"
                class="text-[#1C1C1C] hover:underline hover:text-[rgba(18,127,255,1)]"
                >{{ homeLink[id].name }}</a
              >
              <p
                class="text-[#8B96A5] text-[13px] font-normal"
              >
                {{ homeLink[id].price }}
              </p>
            </div>
          </div>

          <div
            class="hidden sm:flex flex-col justify-center items-center border rounded-lg py-6 w-full"
          >
            <div class="h-[120px]">
              <img :src="homeLink[id + 1].img" alt="" class="w-28 h-28" />
            </div>
            <div class="flex flex-col items-center gap-2 mt-5">
              <a
                href="#"
                class="text-[#1C1C1C] hover:underline hover:text-[rgba(18,127,255,1)]"
                >{{ homeLink[id + 1].name }}</a
              >
              <p
                class="text-[#8B96A5] text-[13px] font-normal"
              >
                {{ homeLink[id + 1].price }}
              </p>
            </div>
          </div>
        </div>
      </div>

      <button
        @click="nextHome"
        :class="
          homeLink.length - 2 == id
            ? 'text-gray-200 text-[50px]'
            : 'text-gray-400 text-[50px]'
        "
      >
        <i class="bx bxs-chevron-right-circle"></i>
      </button>
    </div>
  </div>
</template>

<script setup>
import { ref } from "vue";
import { offerLinks } from "~/store/info/offer";
import { homeLinks_1 } from "~/store/info/home-1";
import { homeLinks_2 } from "~/store/info/home-2";
import { elecLinks_1 } from "~/store/info/electironic-1";
import { elecLinks_2 } from "~/store/info/electironic-2";
import { recItemsLinks } from "~/store/info/rec-items";
import { serviceLinks } from "~/store/info/services";
import { flagLinks } from "~/store/info/flag";
import {homeLinks} from "~/store/info/home"

const offerLink = ref(offerLinks);
const sch = ref(0);
const next = () => {
  if (sch.value == offerLink.value.length - 1) {
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

const id = ref(0);
const nextHome = () => {
  if (id.value == homeLink.value.length - 1) {
    id.value = id.value;
  } else {
    id.value = id.value + 1;
  }
};
const backHome = () => {
  if (id.value == 0) {
    id.value = id.value;
  } else {
    id.value = id.value - 1;
  }
};

const homeLink = ref(homeLinks)

const homeLink_1 = ref(homeLinks_1);
const homeLink_2 = ref(homeLinks_2);

const elecLink_1 = ref(elecLinks_1);
const elecLink_2 = ref(elecLinks_2);

const recItemsLink = ref(recItemsLinks);

const serviceLink = ref(serviceLinks);

const flagLink = ref(flagLinks);

const modal = ref(false);
const toggleModal = () => (modal.value = !modal.value);
</script>

<style lang="scss">
body {
  font-family: "Inter", sans-serif;
  background-color: #f7fafc;
  // font-family: "Roboto", sans-serif;
}
</style>
