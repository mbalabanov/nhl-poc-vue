<template>
  <div class="container border rounded my-2 bg-white">
    <div class="row my-3 py-3">
      <div class="col-md-3 text-center">
        <h3>Player Name:<br />Roger Equidem</h3>
        <p>
          <img
            src="../assets/images/player1.jpg"
            class="img-fluid rounded-circle p-4"
            alt="Player Image"
          />
        </p>
        <h4>Tui montes nascetur.</h4>
        <p>
          Tityre, tu patulae recubans sub tegmine
          fagi dolor. At nos hinc posthac, sitientis piros Afros.
        </p>
      </div>
      <div class="col-md-4">
        <table class="table">
          <tbody>
            <tr>
              <th scope="row">1</th>
              <td>Adelais</td>
              <td>Kvetoslav</td>
              <td>72</td>
            </tr>
            <tr>
              <th scope="row">2</th>
              <td>Krastio</td>
              <td>Girish</td>
              <td>70</td>
            </tr>
            <tr>
              <th scope="row">3</th>
              <td>Avis</td>
              <td>Hedvig</td>
              <td>69</td>
            </tr>
            <tr>
              <th scope="row">4</th>
              <td>Samir</td>
              <td>Lygia</td>
              <td>67</td>
            </tr>
            <tr>
              <th scope="row">5</th>
              <td>Tom</td>
              <td>Pollux</td>
              <td>64</td>
            </tr>
            <tr>
              <th scope="row">6</th>
              <td>Neha</td>
              <td>Gonçal</td>
              <td>63</td>
            </tr>
            <tr>
              <th scope="row">7</th>
              <td>Ayoub</td>
              <td>Hermolaos</td>
              <td>62</td>
            </tr>
            <tr>
              <th scope="row">8</th>
              <td>Blaha Luisa</td>
              <td>Ter</td>
              <td>61</td>
            </tr>
            <tr>
              <th scope="row">9</th>
              <td>Peter</td>
              <td>Jóhann</td>
              <td>60</td>
            </tr>
          </tbody>
        </table>
      </div>
      <div class="col-md-5">
        <vue3-chart-js
          :id="radarChart.id"
          :type="radarChart.type"
          :data="radarChart.data"
          @before-render="beforeRenderLogic"
        ></vue3-chart-js>
      </div>
    </div>
  </div>
</template>

<script>
import Vue3ChartJs from "@j-t-mcc/vue3-chartjs";

export default {
  name: "PlayerRadarChart",
  components: {
    Vue3ChartJs,
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
    const radarChart = {
      id: "radar",
      type: "radar",
      data: {
        labels: [
          "Skating",
          "Puck possession",
          "Defending",
          "Attacking",
          "Falling",
          "Retreating",
          "Standing",
        ],
        datasets: [
          {
            label: "First Dataset",
            data: [65, 59, 90, 81, 56, 55, 40],
            fill: true,
            backgroundColor: "rgba(99, 200, 132, 0.2)",
            borderColor: "rgb(99, 200, 132)",
            pointBackgroundColor: "rgb(59, 155, 32)",
            pointBorderColor: "#fff",
            pointHoverBackgroundColor: "#fff",
            pointHoverBorderColor: "rgb(255, 99, 132)",
          },
          {
            label: "Second Dataset",
            data: [28, 48, 40, 19, 96, 27, 100],
            fill: true,
            backgroundColor: "rgba(54, 162, 235, 0.2)",
            borderColor: "rgb(54, 162, 235)",
            pointBackgroundColor: "rgb(24, 62, 135)",
            pointBorderColor: "#fff",
            pointHoverBackgroundColor: "#fff",
            pointHoverBorderColor: "rgb(54, 162, 235)",
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
      radarChart,
      beforeRenderLogic,
    };
  },
};
</script>

<style scoped>
</style>
