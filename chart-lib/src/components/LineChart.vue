<template>
  <div>
    <canvas id="LineChart"></canvas>
  </div>
</template>

<script>
import Chart from "chart.js";
export default {
    mounted() {
        var ctx = document.getElementById('LineChart').getContext('2d');
        // eslint-disable-next-line
        var chart = new Chart(ctx, {
            type: 'line',
            data: {
                labels: ['January', 'February', 'March', 'April', 'May', 'June', 'July'],
                datasets: [{
                    label: 'My First Dataset',
                    backgroundColor: 'rgb(255, 99, 132)',
                    borderColor: 'rgb(255, 99, 132)',
                    data: [0,10,5,2,20,30,45],
                }]
            },
            options: {}
        });
    }
}
</script>

<style>

</style>