<template>
  <div>
    <chartjs-bar
    :width="600"
    :height="400"
    v-bind:beginzero="beginZero"
    v-bind:labels="labels"
    v-bind:datasets="datasets"
    v-bind:data="data"
    v-bind:fill="fill"
    >
    </chartjs-bar>
  </div>
</template>

<script>
export default {
  data(){
    return{
      beginZero: true,
      datalabel: "Encuesta realizada",
      labels: "",
      fill: true,
      datasets: [{
				label: 'SI',
				backgroundColor: 'blue',
				borderColor: 'black',
				borderWidth: 1,
				data: [
					10
				]
      }, 
      {
				label: 'NO',
        backgroundColor: 'red',
				borderColor: 'black',
				data: [12]
      },
       {
				label: 'NO ME INTERESA',
        backgroundColor: 'orange',
				borderColor: 'black',
				data: [6]
      }
      ]

    }
  }
};
</script>


