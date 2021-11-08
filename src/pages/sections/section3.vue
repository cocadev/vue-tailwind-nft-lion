<template>
  <section class="bg-gray-500 py-8 px-4 lg:px-12 lg xl:py-12 2xl:py-16 Home_section4__3tiCo" id="roadSection">
    <div class="max-w-7xl mx-auto relative z-40">
      <div class="text-center">
        <h2 class="font-bold font-serif text-2xl md:text-3xl lg:text-4xl xl:text-6xl 2xl:text-7xl">
          <span class="text-yellow-300">The Roadmap </span>
        </h2>
        <p class="mt-4 text-white lg:text-xl lg:mt-4 xl:mt-6 xl:max-w-2xl 2xl:text-3xl 2xl:max-w-5xl 2xl:mt-8 mx-auto">
          Every Lazy Lion comes with exclusive access to the private island.
        </p>
      </div>
      <div class="mt-8 lg:mt-10 xl:mt-12 pr-2">
        <div class="relative mt-8 lg:mt-10 xl:mt-12 2xl:mt-8" v-for="(i, index) in roadmaps" :key="index">
          <div class="relative z-20 bg-blue-300 py-6 px-8 rounded-tr-2xl rounded-bl-2xl xl:py-8 xl:px-10 2xl:py-10 2xl:px-12">
            <p class="font-bold text-lg md:text-xl lg:text-2xl xl:text-3xl 2xl:text-4xl">
              {{i.title}}
            </p>
            <div v-for="(x, key) in i.descriptions" :key="key">
              <p class="text-white font-bold text-lg md:text-xl lg:text-2xl xl:text-3xl 2xl:text-4xl mt-3 lg:mt-4 2xl:mt-6">
                {{x.note}}
              </p>
              <p class="mt-1 lg:text-xl 2xl:text-3xl">
                {{x.guide}}
              </p>
            </div>
          </div>
          <div class="bg-yellow-300 w-full h-full absolute top-2 left-2 md:top-3 md:left-3 rounded-tr-5xl rounded-bl-5xl z-10" />
        </div>
      </div>
    </div>
  </section>
</template>

<script>
export default {
  name: "Section3",
  data(){
    return {
      roadmaps: [
        { 
          title: '0% The Jetty is open. Welcome to the island of KINGS!',
          descriptions: [
            {
              note: 'The private island is open.',
              guide: 'The private discord channel will be available exclusively for Lazy Lion owners.'
            }
          ]  
        },
        {
          title: '20% The community wallet is opened.',
          descriptions: [
            {
              note: 'We have opened a tab at the Cabana Bar for all Lazy Lion owners to enjoy.',
              guide: 'The community wallet will be used for a variety of things for ensuring longevity.'
            },
            {
              note: 'Hit the gym where hard work gets rewarded…',
              guide: 'Community rewards for Lazy Lions engaged up in Discord.'
            }
          ]  
        },
        {
          title: '40% ROARwards Program available to all Lazy Lion holders.',
          descriptions: [
            {
              note: 'The Buffet is open and everyone’s invited.',
              guide: 'Lazy Lion holders are eligible to participate in a program that rewards community engagement.'
            },
            
          ]  
        },
        {
          title: '60% Exclusive merch drop.',
          descriptions: [
            {
              note: 'The Shopping Strip is now open.',
              guide: 'Get decked out in an exclusive selection of Lazy Lion merch.'
            },
            {
              note: 'Get the VIP Spa treatment.',
              guide: 'Lazy Lion owners with a selected trait (to be revealed) will receive free merch.'
            }
          ]  
        },
        {
          title: '80% New NFTs free for all Lazy Lions!',
          descriptions: [
            {
              note: 'The Bungalows are open and every Lazy Lion gets one!',
              guide: 'Every Lazy Lion owner can receive a banner image NFT featuring their own unique, randomly generated private bungalow!'
            }
          ]  
        },
        {
          title: '100% Lazy Lions Game… Play-to-earn!',
          descriptions: [
            {
              note: '',
              guide: 'An exclusive Lazy Lions play-to-earn game will be released with community prizes.'
            }
          ]  
        }
      ]
    }
  }
};
</script>