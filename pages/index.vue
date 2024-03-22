<template>
  <section class="flex flex-col">
    <div class="h-[50vh] home-banner flex flex-col justify-center pl-10 gap-5">
      <p class="text-4xl md:text-6xl text-white w-full md:max-w-[80vw]">
        Welcome to Knowledge Kinetics Organization (2KO)
      </p>
      <button class="p-3 md:p-4 bg-[#1F2223] text-white rounded-lg w-max text-md md:text-xl">
        About Us
      </button>
    </div>
  </section>

  <Services />
  <Standards />
  <KnowledgeBanner />
</template>

<style>
.home-banner {
  background-image: url("/images/hero.png");
  background-size: cover;
  background-position: center;
  background-repeat: no-repeat;
}
</style>