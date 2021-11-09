<template>
    <footer class="bg-yellow-600 px-4 lg:px-12 lg py-8 md:py-0 relative Home_footer__1WdhD">
      <div class="relative z-30 max-w-7xl mx-auto">
        <div class="flex items-end justify-between">
          <div class="hidden md:flex">
            <img :src="white" />
            <img
              alt="lion"
              src="../assets/images/lion.png"
              decoding="async"
              data-nimg="intrinsic"
              class="absolute top-0"
            />
          </div>
          <div class="bg-gray-500 text-white font-serif py-6 px-10 w-11/12 mx-auto md:ml-auto md:mr-0 self-center md:w-5/6 lg:w-3/6">
            <p class="text-base md:text-lg lg:text-xl xl:text-2xl 2xl:text-2xl">
              VERIFIED SMART CONTRACT:
            </p>
            <p class="text-lg mx:auto md:text-xl lg:text-2xl xl:text-3xl 2xl:text-2xl font-bold text-green-300">
              <a :href='link'>View on Etherscan</a>
            </p>
            <div class="w-32 bg-yellow-300 my-6 lg:my-8" style="height: 2px"></div>
            <span>Privacy Policy</span>
            |
            <span>Terms of Sale</span>
          </div>
        </div>
      </div>
      <p class="xl:text-xl md:absolute bottom-2 left-1/2 transform md:-translate-x-1/2 text-white text-center mt-3 md:mt-0">
        © 2021 Blockchain Media Pty Ltd
      </p>
    </footer>
</template>

<script>
export default {
  name: 'Footer',
  data(){
    return {
      white: 'data:image/svg+xml;base64,PHN2ZyB3aWR0aD0iNDAwIiBoZWlnaHQ9IjQwMCIgeG1sbnM9Imh0dHA6Ly93d3cudzMub3JnLzIwMDAvc3ZnIiB2ZXJzaW9uPSIxLjEiLz4=',
      link: 'https://etherscan.io/address/0x8943c7bac1914c9a7aba750bf2b6b09fd21037e0'
    }
  }
}
</script>