<script>
import { Pie } from 'vue-chartjs'

export default Pie.extend({
  mounted () {
    this.renderChart({
      labels: ['Type I', 'Type II', 'Type III'],
      datasets: [
        {
          backgroundColor: [
            '#41B883',
            '#E46651',
            '#00D8FF'
          ],
          data: [70, 20, 10]
        }
      ]
    }, {responsive: true, maintainAspectRatio: false})
  }
})
</script>
