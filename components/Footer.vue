<template>
  <section class="p-10 bg-[#1F2223]  text-white flex flex-col gap-10">
    <div class="flex flex-col justify-between w-full gap-10 md:flex-row md:gap-0">
      <div class="flex flex-col gap-4 ">
        <p class="text-xl">Contact Information</p>
        <ul class="flex flex-col gap-4">
          <li class="flex items-center gap-2">
            <Icon name="basil:phone-solid" size="1.5rem" />
            <p>0548021100 / 0248095665</p>
          </li>
          <li class="flex items-center gap-2">
            <Icon name="basil:envelope-solid" size="1.5rem" />
            <p>knowledgekinetics.gh@gmail.com</p>
          </li>
          <li class="flex items-center gap-2">
            <Icon name="basil:home-solid" size="1.5rem" />
            <p>5 Kpetenkplebi Street Dzorwulu - Accra Ghana</p>
          </li>
        </ul>
      </div>
      <div class="flex flex-col gap-4">
        <p class="text-xl">Subscribe to Our Newsletter</p>
        <form class="flex flex-col gap-3">
          <input type="email" placeholder="Enter your email" class="w-full p-2 bg-white rounded-md" />
        <button class="bg-white text-[#1F2223] rounded-md p-2 w-max">Subscribe</button>
      </form>
      </div>
    </div>
    <div class="flex justify-between w-full gap-10 md:flex-row md:gap-0">
      <div><img src="/images/logo.png" alt=""></div>
      <div class="flex items-center self-end gap-3 ml-auto">
      <Icon name="basil:facebook-solid" size="1.5rem" />
      <Icon name="basil:twitter-solid" size="1.5rem" />
      <Icon name="basil:instagram-solid" size="1.5rem" />
      <Icon name="basil:youtube-solid" size="1.5rem" />
    </div>
    </div>
    <div class="w-full border-t border-white"></div>
    <p>Copyright © 2024 Knowledge Kinetics Organization</p>
  </section>
</template>

