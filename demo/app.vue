<template>
  <div>
  	<p>
  		Here is the demo of vue-fullcalendar, no jquery fullcalendar.js required!
  	</p>
    <full-calendar class="test-fc" :events="fcEvents" lang="en"></full-calendar>
  </div>
</template>
<script>
let demoEvents = [
    {
      title : 'Sunny 728-730',
      start : '2016-07-25',
      end : '2016-07-27'
    },
    {
      title : 'Sunny 726-727',
      start : '2016-07-26',
      end : '2016-07-27'
    },
    {
      title : 'Sunny 727-728',
      start : '2016-07-27',
      end : '2016-07-28'
    },
    {
      title : 'Sunny 728-730',
      start : '2016-07-28',
      end : '2016-07-30'
    },
  ]

export default {
	data () {
		return {
      name:'Sunny!',
      fcEvents : demoEvents
    }
	},
  components : {
    'full-calendar' : require('src/fullCalendar')
  }
}
</script>
<style lang='scss'>
  .app{
    color:green;
  }
</style>