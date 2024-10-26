<template>
  <div class="text-left">
    <div class="mb-3 ">
      <h2 v-if="givers !== undefined" class="font-bold text-4xl">
        {{ givers }}
      </h2>
      <v-progress-circular v-else indeterminate :size="40" />
      <p>Givers</p>
    </div>

<!--	  <div class="py-3">
		  <h2 class="font-bold text-4xl">{{daysRemaining}}</h2>
		  <p>Days to Go</p>
	  </div>-->
  </div>
</template>

<script>
export default {
  name: 'DisplayNumbers',
  props: {
    givingAmount: {
      type: Number,
      required: false,
      default: undefined,
    },
    givingGoal: {
      type: Number,
      required: true,
    },
    givers: {
      type: Number,
      required: false,
      default: undefined,
    },
  },
  computed: {
    daysRemaining() {
      const today = new Date();
      const end = new Date("2024-06-01");
      const millisecondsInDay = 1000*60*60*24;
      const diff = end.getTime() - today.getTime();
      return Math.ceil(diff / millisecondsInDay);
    }
  },
}
</script>
