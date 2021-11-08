<template>
  <section class="bg-yellow-600 py-8 pl-4 pr-6 lg:pr-12 lg:pl-10 lg xl:py-12 2xl:py-16 Home_section3__3OhR8">
    <div class="max-w-screen-2xl mx-auto relative z-20">
      <div class="flex flex-col items-center md:flex-row">
        <div class="relative flex flex-col" style="max-width: 400px">
          <div>
            <div class="relative z-30 bg-gray-900 w-full p-3 rounded-tr-3xl rounded-bl-3xl">
              <div class="flex flex-wrap">
                <div class="w-1/2 p-2" v-for="(i, index) of lions" :key="index">
                  <span class="relative inline-block">
                    <img :src="white" />
                    <img
                      alt="lion"
                      :src="getImgUrl(i.img)"
                      decoding="async"
                      data-nimg="intrinsic"
                      class="bg-blue-400 rounded-tr-xl rounded-bl-xl absolute top-0"
                    />
                  </span>
                </div>
              </div>
            </div>
            <div class="bg-green-300 w-full h-full absolute top-2 left-2 md:top-3 md:left-3 rounded-tr-5xl rounded-bl-5xl z-10"/>
          </div>
        </div>
        <div class="text-center font-serif max-w-md md:text-left md:w-auto md:max-w-full md:flex-1 md:ml-auto md:pl-5 lg:pl-16 xl:max-w-4xl 2xl:max-w-5xl mt-8 md:mt-0">
          <h1 class="font-bold font-serif text-2xl md:text-3xl lg:text-4xl xl:text-6xl 2xl:text-7xl">
            <span class="text-green-300">Rarity</span>
          </h1>
          <h2 class="mt-2 font-bold text-xl text-white lg:text-2xl lg:mt-4 xl:mt-6 xl:text-4xl 2xl:mt-8 2xl:text-5xl">
            Every lion is a KING.
          </h2>
          <p class="mt-4 text-white lg:text-xl lg:mt-4 xl:mt-6 xl:max-w-2xl 2xl:text-3xl 2xl:max-w-5xl 2xl:mt-8">
            Each Lazy Lion is unique and programmatically generated from over
            160 possible traits, including clothing, mane, expression, and more.
          </p>
        </div>
      </div>
    </div>
  </section>
</template>

<script>
export default {
  name: "Section2",
  data(){
    return{
      white: 'data:image/svg+xml;base64,PHN2ZyB3aWR0aD0iMjAwIiBoZWlnaHQ9IjIwMCIgeG1sbnM9Imh0dHA6Ly93d3cudzMub3JnLzIwMDAvc3ZnIiB2ZXJzaW9uPSIxLjEiLz4=',
      lions: [
        { img: 'lion1.jpg' },
        { img: 'lion2.jpg' },
        { img: 'lion3.jpg' },
        { img: 'lion4.jpg' },
      ],
      getImgUrl(pic) {
        return require('../../assets/images/'+ pic)
      },
    }
  }
};
</script>