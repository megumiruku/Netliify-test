<template>
  <div class="card">
    <img class="card-img" src="https://coachtech-video.s3-ap-northeast-1.amazonaws.com/clouds-449822_640.jpg"/>
    <div class="card-content">
      <h1 class="card-title">{{city}}</h1>
    </div>
    <div class="card-link">
      <a @click="$router.push({name:'About', params: {city:city}})">About</a>
    </div>
  </div>
</template>

<script>
export default {
  props: ["city"],
};
</script>

<style>
.card {
  width: 27%;
  margin:30px;
  background: #fff;
  border-radius: 5px;
  box-shadow: 0 2px 5px #ccc; 
}
.card-img {
  border-radius: 5px 5px;
  max-width: 100%;
  height: auto;
}
.card-content {
  padding: 20px;
}
.card-title {
  font-size: 20px;
  /* margin-bottom: 20px; */
  text-align: center;
  color:#333;
}
.card-link {
  text-align: center;
  border-top: 1px solid #eee;
  padding:20px;
}
.card-link a {
  text-decoration: none;
  cursor: pointer;
  margin: 0 10px;
  color: #0bd;
}
.card-link a:hover {
  color:#0090aa;
}

</style>