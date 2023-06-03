<template>
  <div class="container mx-auto px-5 py-5">
    <div
      class="mt-32 flex items-center justify-between gap-5 border border-[#DEE2E7] rounded-lg p-5 mb-5"
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

    <div class="flex border border-[#DEE2E7] rounded-lg mb-5">
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

    <div class="border border-[#DEE2E7] rounded-lg flex w-[100%] mb-5">
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
            <h3>{{ home.name }}</h3>
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
            <h3>{{ hom.name }}</h3>
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

    <div class="border border-[#DEE2E7] rounded-lg flex w-[100%] mb-5">
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
            <h3>{{ elec.name }}</h3>
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
            <h3>{{ elek.name }}</h3>
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
      class="rounded-lg flex w-[100%] bg-no-repeat bg-cover bg-center bg-[url('/store/img/img/Group982.png')] p-10 justify-between"
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
        <input type="text" placeholder="What item you need?" class="outline-none border rounded-lg w-full p-2 mb-3"/>
        <textarea name="" id="" cols="30" rows="10" placeholder="Type more details" class="outline-none border p-2 rounded-lg w-full h-[73px] mb-2"></textarea>
        <div class="flex items-center mb-5">
          <input type="text" placeholder="Quantity" class="outline-none border rounded-lg p-2"/>

        </div>
        <button class="bg-[rgba(18,127,255,1)] text-white rounded-lg border border-[rgba(18,127,255,1)] px-4 py-2 hover:bg-white hover:text-[rgba(18,127,255,1)]">
          Send inquiry
        </button>
      </div>
    </div>
  </div>
</template>

<script setup>
import { offerLinks } from "~/store/info/offer";
import { homeLinks_1 } from "~/store/info/home-1";
import { homeLinks_2 } from "~/store/info/home-2";
import { elecLinks_1 } from "~/store/info/electironic-1";
import { elecLinks_2 } from "~/store/info/electironic-2";

const offerLink = ref(offerLinks);

const homeLink_1 = ref(homeLinks_1);
const homeLink_2 = ref(homeLinks_2);

const elecLink_1 = ref(elecLinks_1);
const elecLink_2 = ref(elecLinks_2);
</script>

<style lang="scss"></style>
