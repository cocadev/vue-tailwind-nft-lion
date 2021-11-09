<template>
    <header class="Home_header__3vlZW w-full relative">
      <nav class="flex flex-col w-full h-full md:h-auto md:flex-row md:justify-start max-w-screen-2xl px-4 items-center justify-center mx-auto md:py-8 xl:py-12 2xl:py-16">
        <ul class="flex flex-col items-center mt-2 md:h-full md:mt-0 md:ml-auto md:flex-row justify-center md:justify-start">
          <div class="flex items-center w-full md:w-auto justify-center md:justify-start">
            <li v-for="(i, index) in links" :key="index" :class="i.class">
              <a
                :href="i.href"
                target="_blank"
                rel="noreferrer"
              >
                <span class="block mr-7 text-2xl font-bold text-black border-b-4 border-black cursor-pointer" duration="500">{{i.title}}</span>
              </a>
            </li>
          </div>
        </ul>
      </nav>
      <div class="hidden md:block w-6 h-12 rounded-3xl absolute bottom-10 left-1/2 transform -translate-x-1/2 z-20 Home_scrollDownButton__2F7UY py-1 lion-scroll-bar" />
    </header>
</template>

<style scoped>
 .lion-scroll-bar {
   box-shadow: inset 0 0 0 1px rgb(0 0 0 / 50%)
 }
</style>

<script>
export default {
  name: 'Header',
  data(){
    return{
      links: [
        { link: 'https://roarwards.lazylionsnft.com/', title: 'ROARwards', class: '' },
        { link: 'https://bungalows.lazylionsnft.com/', title: 'Bungalows', class: 'hidden md:block' },
        { link: '', title: 'About', class: 'hidden md:block' },
        { link: '', title: 'Roadmap', class: 'hidden md:block' }
      ]
    }
  }
}
</script>