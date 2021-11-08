<template>
  <section class="bg-gray-500 py-8 pl-4 pr-6 lg:pr-12 lg:pl-10 lg xl:py-12 2xl:py-16 Home_section1__1zJmv" id="aboutSection">
    <div class="max-w-screen-2xl mx-auto relative z-20">
      <div class="flex flex-col items-center md:flex-row">
        <div class="relative flex flex-col md:order-2" style="max-width: 400px">
          <img :src="white" />
          <img
            alt="lion"
            src="../../assets/images/liongif.gif"
            decoding="async"
            data-nimg="intrinsic"
            class="z-20 bg-blue-400 rounded-tr-5xl rounded-bl-5xl absolute top-0"
          />
          <div class=" bg-green-300 w-full h-full absolute top-2 left-2 md:top-3 md:left-3 z-10 rounded-tr-5xl rounded-bl-5xl" />
        </div>
        <div class=" text-center font-serif max-w-md md:text-left md:w-auto md:max-w-full md:flex-1 md:mr-auto md:pr-5 lg:pr-16 xl:max-w-4xl 2xl:max-w-5xl">
          <h1 class="mt-6 font-bold font-serif text-2xl md:text-3xl md:mt-8 lg:text-4xl xl:text-7xl 2xl:text-8xl">
            <span class="text-green-300">Welcome to Lazy Lions </span>
            <span class="text-blue-300"> Private Island </span>
          </h1>
          <h2 class="mt-2 font-bold text-xl text-white lg:text-2xl lg:mt-6 xl:mt-10 xl:text-4xl 2xl:mt-12 2xl:text-5xl">
            The island made for kings!
          </h2>
          <p class="mt-4 text-white lg:text-xl lg:mt-6 xl:mt-10 xl:max-w-2xl 2xl:text-3xl 2xl:max-w-5xl 2xl:mt-12">
            Located in a secured, top-secret location, this private island is
            open exclusively for the VIP members of the Lazy Lion Community.
          </p>
          <p class="mt-4 text-white lg:text-xl lg:mt-6 xl:mt-10 xl:max-w-2xl 2xl:text-3xl 2xl:max-w-5xl 2xl:mt-12">
            Hosted on the Ethereum blockchain.
          </p>
        </div>
      </div>
    </div>
  </section>
</template>

<script>
export default {
  name: "Section1",
  data(){
    return{
      white: 'data:image/svg+xml;base64,PHN2ZyB3aWR0aD0iNDAwIiBoZWlnaHQ9IjQwMCIgeG1sbnM9Imh0dHA6Ly93d3cudzMub3JnLzIwMDAvc3ZnIiB2ZXJzaW9uPSIxLjEiLz4='
    }
  }
};
</script>