<template>
  <div>
    <div class="text-center mx-auto">
      <div class="mx-auto text-center lg:max-w-7xl pb-10">
        <div class="grid grid-cols-12 gap-4 md:px-5">

          <div class="col-span-12 md:col-span-7 md:order-2">
            <VideoPlayer/>
          </div>

          <div class="col-span-12 md:order-1">
            <div class="mt-2 md:pt-14 pb-14 p-2 text-left md:text-center mx-auto">
              <h1 class="uppercase font-bold text-4xl">Foothills Church Vision Offering</h1>
              <p class="bold text-2xl">Together we can take our next step as a church by giving to the vision offering.</p>
            </div>
          </div>


          <div class="col-span-12 md:col-span-5 md:order-3">
            <div class="px-2 lg:px-10">
              <GivingData/>
              <XLButton/>
            </div>
          </div>
        </div>
      </div>

      <FullBanner/>

    </div>

    <v-card>
      <div class="text-center mx-auto">
        <div class="mx-auto text-left px-5 md:max-w-7xl md:mx-auto pt-5">

          <v-tabs
            v-model="tab"
            align-with-title
          >
            <v-tabs-slider></v-tabs-slider>
            <v-tab key="Campaign">Campaign</v-tab>
            <v-tab key="FAQ">FAQ</v-tab>
          </v-tabs>


          <v-tabs-items v-model="tab">
            <v-tab-item key="Campaign">
              <CampaignTab/>
            </v-tab-item>
            <v-tab-item key="FAQ">
              <FaqTab/>
            </v-tab-item>
          </v-tabs-items>
        </div>
      </div>
    </v-card>

  </div>
</template>

<script>
export default {
  name: 'IndexPage',
  data() {
    return {
      tab: null,
    }
  },
  head() {
    return {
      title: "Foothills Church Vision Offering 2023",
      meta:[
        { hid: 'og-type', property: 'og:type', content: 'The Vision Offering 2023' },
        { hid: 'og-desc', property: 'og:description', content: 'Together we can take our next step as a church by giving to the vision offering.' },
        { hid: 'og-image', property: 'og:image',
          content: '/images/vo-main.jpg'
        },
      ]
    };
  },
}
</script>
