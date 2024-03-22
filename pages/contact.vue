<template>
<section class="flex flex-col gap-10 p-10">
    <div class="flex flex-col w-full h-full gap-5">
        <p class="text-2xl font-semibold">Reach Out to Us</p>
        <div class="flex flex-col w-full h-full gap-5 lg:flex-row lg:justify-between lg:gap-0">
            <form class="w-full lg:w-[40%] flex-col flex gap-5">
                <div class="flex flex-col gap-1">
                    <label for="name">Full Name</label>
                    <input type="text" placeholder="Enter your full name" class="w-full p-2 bg-white border-2 rounded-md" />
                </div>
                <div class="flex flex-col gap-1">
                    <label for="Phone">Phone Number</label>
                    <input type="tel" placeholder="Enter your phone number" class="w-full p-2 bg-white border-2 rounded-md" />
                </div>
                <div class="flex flex-col gap-1">
                    <label for="message">Message</label>
                    <textarea placeholder="Enter your message" class="w-full p-2 bg-white border-2 rounded-md"></textarea></div>
                <button class="text-white bg-[#1F2223] rounded-md p-2 w-max">Submit</button>
            </form>
            <div class="w-full lg:w-[50%] h-[40vh] ">
              <div class="mapouter"><div class="gmap_canvas"><iframe class="gmap_iframe" frameborder="0" scrolling="no" marginheight="0" marginwidth="0" src="https://maps.google.com/maps?width=600&amp;height=400&amp;hl=en&amp;q=5 Kpetenkplebi Street Dzorwulu&amp;t=&amp;z=14&amp;ie=UTF8&amp;iwloc=B&amp;output=embed"></iframe><a href="https://strandsgame.net/">Strands NYT</a></div></div>
            </div>
        </div>
    </div>

</section>
</template>


<style scoped>
.mapouter {
    position: relative;
    text-align: right;
    @apply w-full h-full;
}

.gmap_canvas {
    overflow: hidden;
    background: none !important;
    @apply w-full h-full;
}

.gmap_iframe {
    @apply w-full h-full;
}
</style>