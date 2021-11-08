<template>
  <section class="bg-yellow-300 py-8 px-4 lg:px-12 lg xl:py-12 2xl:py-16 Home_section5__3vq1Y">
    <h2 class="font-bold font-serif text-3xl md:text-4xl lg:text-4xl xl:text-6xl 2xl:text-7xl text-center mb-8">
      <span class="text-black">Team</span>
    </h2>
    <div class="flex flex-col items-center -my-2 -mx-2 md:flex-row justify-center relative z-30">
      <a target="_blank" rel="noreferrer" v-for="i in lions" :key="i.id" :href="getLink(i.link)">
        <div class="2xl:max-w-xs py-2 px-2 lex flex-col items-center cursor-pointer Home_lionButton__1HRuZ">
          <div class=" border-4 border-blue-300 w-full rounded-tr-3xl rounded-bl-3xl flex overflow-hidden">
            <div class="relative inline-block">
              <img :src="white"/>
              <img
                alt="lion"
                :src="getImgUrl(i.img)"
                decoding="async"
                data-nimg="intrinsic"
                class="bg-blue-400 top-0 absolute"
              />
            </div>
          </div>
          <p class="mt-4 lg:mt-6 text-2xl lg:text-3xl xl:text-4xl 2xl:text-5xl font-bold font-serif text-center">
            {{i.name}}
          </p>
        </div> 
        </a>
    </div>
  </section>
</template>

<script>
export default {
  name: "Section4",
  data() {
    return {
      white: 'data:image/svg+xml;base64,PHN2ZyB3aWR0aD0iMzAwIiBoZWlnaHQ9IjMwMCIgeG1sbnM9Imh0dHA6Ly93d3cudzMub3JnLzIwMDAvc3ZnIiB2ZXJzaW9uPSIxLjEiLz4=',
      lions: [
        { id: 1, name: 'Ashur', img: "lion_ashur.jpg", link: 'AshurNft'},
        { id: 2, name: 'Anlion', img: "lion_anlil.jpg", link: 'LazyLionAnlion'},
        { id: 3, name: 'Nine', img: "lion_nine.jpg", link: 'NineNft'},
        { id: 4, name: 'Nin', img: "lion_nin.jpg", link: 'NinLioness'},
      ],
      getImgUrl(pic) {
        return require('../../assets/images/'+ pic)
      },
      getLink(link) {
        return 'https://twitter.com/'+ link
      }
    };
  },
};
</script>