<template>
  <div class="container border rounded my-2 bg-white">
    <div class="row my-3 py-3">
      <div class="col-md-3 text-center">
        <h3>Player Name:<br>Jim Legentibus</h3>
        <p>
          <img
            src="../assets/images/player2.jpg"
            class="img-fluid rounded-circle p-4"
            alt="Player Image"
          />
        </p>
        <h4>Sum ceteris in veneratione.</h4>
        <p>
          Filtum, deserunt mollit anim laborum astutumque! Salutantibus vitae
          elit libero, a pharetra augue.
        </p>
      </div>
      <div class="col-md-4">
        <table class="table">
          <tbody>
            <tr>
              <th scope="row">1</th>
              <td>Mark</td>
              <td>Otto</td>
              <td>62</td>
            </tr>
            <tr>
              <th scope="row">2</th>
              <td>Jacob</td>
              <td>Thornton</td>
              <td>61</td>
            </tr>
            <tr>
              <th scope="row">3</th>
              <td>Larry</td>
              <td>Smith</td>
              <td>60</td>
            </tr>
            <tr>
              <th scope="row">4</th>
              <td>Kevin</td>
              <td>Anderson</td>
              <td>59</td>
            </tr>
            <tr>
              <th scope="row">5</th>
              <td>John</td>
              <td>Kozlowski</td>
              <td>58</td>
            </tr>
            <tr>
              <th scope="row">6</th>
              <td>Steve</td>
              <td>Chomsky</td>
              <td>56</td>
            </tr>
            <tr>
              <th scope="row">7</th>
              <td>Jeff</td>
              <td>Streetson</td>
              <td>56</td>
            </tr>
            <tr>
              <th scope="row">8</th>
              <td>Tom</td>
              <td>Winston</td>
              <td>55</td>
            </tr>
          </tbody>
        </table>
      </div>
      <div class="col-md-5">
        <vue3-chart-js
          :id="doughnutChart.id"
          :type="doughnutChart.type"
          :data="doughnutChart.data"
          @before-render="beforeRenderLogic"
        ></vue3-chart-js>
      </div>
    </div>
  </div>
</template>

<script>
import Vue3ChartJs from '@j-t-mcc/vue3-chartjs'

export default {
  name: "PlayerDonutChart",
  components: {
    Vue3ChartJs
  },
  props: {
    type: {
      type: String,
      required: true,
    },
    data: {
      type: Object,
      required: true,
    },
    options: {
      type: Object,
      default() {
        return {};
      },
    },
    plugins: {
      type: Array,
      default() {
        return [];
      },
    },
  },
  setup() {
    const doughnutChart = {
      id: "doughnut",
      type: "doughnut",
      data: {
        labels: ["Time", "Energy", "Possession", "Speed"],
        datasets: [
          {
            backgroundColor: ["#E1F5FE", "#B3E5FC", "#81D4FA", "#4FC3F7"],
            data: [40, 20, 80, 10],
          },
        ],
      },
    };

    const beforeRenderLogic = (event) => {
      //...
      //if(a === b) {
      //  event.preventDefault()
      //}
    };

    return {
      doughnutChart,
      beforeRenderLogic,
    };
  },
};
</script>

<style scoped>
</style>
