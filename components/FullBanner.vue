<template>
  <div class="bg-gray">
    <div class="mx-auto text-center lg:max-w-7xl py-5 px-5">
      <div class="grid grid-cols-12 gap-4 -ml-3 md:ml-0">

        <div class="col-span-12 lg:col-span-4 opacity-20">
          <div class="box">
            <img
              src="/images/icons/heart.png"
              alt="icon"
              class="icon-width m-3"
            >
            <span class="text-left"><strong>COMPLETED: Goal #1 - $94,500</strong> <br />Bless Outreach Minisries</span>
          </div>
        </div>

        <div class="col-span-12 lg:col-span-4">
          <div class="box">
            <img
				src="/images/icons/counsel.png"
              alt="icon"
              class="icon-width m-3"
            >
            <span class="text-left"><strong>CURRENT: Goal #2 - $1,200,000</strong> <br />Build Counseling Center </span>
          </div>
        </div>
      </div>
    </div>
  </div>
</template>

<script>
export default {
  name: 'FullBanner'
}
</script>
