<template>
  <div class="nasa">
    <div class="container">
      <div class="row">
        <div class="col col-3">
          <b-card>
            Astrophotographer : <br>
           <h5> {{ listdata.copyright }} </h5>
          </b-card><br>
        </div>
        <div class="col col-6">
          <b-card>
            <h3>{{ listdata.title }}</h3>
          </b-card>
        </div>
        <div class="col col-3">
          <b-card> Date : {{ listdata.date }} </b-card>
        </div>
        <div class="col col-12">
          <b-card img-top>
            <img v-bind:src="listdata.url" alt="" />
            <b-card-text>
               <br><h5>{{listdata.explanation}}</h5>
            </b-card-text>
          </b-card>
        </div>
      </div>
    </div>
  </div>
</template>

<script>
import axios from "axios";
export default {
  data() {
    return {
      listdata: {},
    };
  },
  mounted() {
    let url = "https://api.nasa.gov/planetary/apod?api_key=DEMO_KEY";
    axios
      .get(url)
      .then((response) => {
        this.listdata = response.data;
      })
      .catch((err) => {
        console.log(err);
      });
  },
};
</script>