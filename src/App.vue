<template>
  <Costumers />
  <Data />
</template>

<script>
import Data from "./components/Data.vue";
import Costumers from "./components/Costumers.vue";

export default {
  name: "App",
  components: {
    Data,
    Costumers,
  },
  data() {
    return {
      costumers: [],
    };
  },
  methods: {
    showData() {
      console.log(this.costumers);
    },
  },
  created() {
    this.costumers = [
      {
        id: 1,
        name: "Sylvia",
        userId: "3647321",
        email: "sylvia123@email.com",
        profilePhoto: "",
        timeZone: "Pacific Time",
        currentSing: "11/05/2020 12:48",
        active: false,
      },
      {
        id: 2,
        name: "Robin",
        userId: "2948922",
        email: "robin@email.com",
        profilePhoto: "",
        timeZone: "Eastern European Time",
        currentSing: "01/02/2010 11:32",
        active: false,
      },
      {
        id: 3,
        name: "Joyce",
        userId: "8156129",
        email: "joyce456@email.com",
        profilePhoto: "",
        timeZone: "European Central Time",
        currentSing: "25/11/2018 09:28",
        active: false,
      },
      {
        id: 4,
        name: "Ting",
        userId: "6166563",
        email: "tingtong@email.com",
        profilePhoto: "",
        timeZone: "Solomon Time",
        currentSing: "12/08/2015 13:10",
        active: false,
      },
    ];
  },
};
</script>

<style>
body {
  background-color: rgb(232, 247, 243);
}
#app {
  width: 90%;
  display: flex;
  font-family: "Open Sans", sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #2c3e50;
  margin-left: 5%;
  margin-right: 5%;
  margin-top: 60px;
  border-radius: 5%;
  background-color: rgba(255, 255, 255, 0.5);
}
/* Colors:
rgb(232,247,243) FONDO */
</style>