<template>
  <div>
    <CanvasJSChart :options="options" />
  </div>
</template>

<script>
export default {
  data() {
    return {
      chart: null,
      options: {
        // animationEnabled: true,
        // exportEnabled: true,
        theme: 'light1',
        title: {
          text: 'December 2023'
        },
        data: [
          {
            type: 'doughnut',
            innerRadius: '95%',
            // showInLegend: true,
            // legendText: '{name}: {y}',
            // yValueFormatString: "#,###'%'",
            dataPoints: [
              { name: 'Scheduled', y: 27, color: '#cbf3f5' },
              { name: 'Delivered', y: 55, color: '#25ced9' },
              { name: 'Cancelled', y: 18, color: '#f72564' }
            ]
          }
        ]
      }
    }
  }
}
</script>
