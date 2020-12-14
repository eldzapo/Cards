<template>
    <div class="card">
        <img :src="image" class="card-image" >

        <div class="card-text">
            <span class="date">4 days ago</span>
            <h2>Post One</h2>
            <p>Lorem ipsum dolor sit amet consectetur, Ducimus, repudiandae temporibus omnis illum maxime quod deserunt eligendi dolor</p>
        </div>
        <div class="button">
            <p>Hello!</p>
        </div>
</div>

</template>


<script>
export default {
    data () {
  return {
    image: require('@/assets/mma1.png')
  }
}


}
</script>


<style scoped>

.card {
  display: inline-block;
  width: 300px;
  height:480px;
  grid-template-columns: 300px;
  grid-template-rows: 210px 210px 80px;
  grid-template-areas: "image" "text" "stats";
  border-radius: 18px;
  background: white;
  box-shadow: 5px 5px 15px 5px rgba(0,114,250,0.38);
  font-family: roboto;
  text-align: center;
  margin-top:200px;
}

.card-image {
  grid-area: image;
}
.card-text {
  grid-area: text;
}
.card-stats {
  grid-area: stats; 
}

.card-image {
  display:inline-block;
  background:'image';
  border-top-left-radius: 15px;
  border-top-right-radius: 15px;
  height:180px;
  width: 100%;
  background-size: cover;
}
.card-text {
  grid-area: text;
  display: inline-block;
  object-position: bottom;
  margin: 20px;
}
.card-text .date {
  color: rgb(255, 7, 110);
  font-size:12px;
}
.card-text p {
  color: grey;
  font-size:15px;
  font-weight: 300;
}
.card-text h2 {
  margin-top:0px;
  font-size:22px;
}

.card-stats {
  grid-area: stats; 
  display: grid;
  position: relative;
  bottom: 0px;
  height: 70px;
  justify-content: grid-row;
  grid-template-columns: 1fr 1fr 1fr;
  grid-template-rows: 1fr;
  border-bottom-left-radius: 15px;
  border-bottom-right-radius: 15px;
  background: rgb(255, 7, 110);
  text-align: center;
}

.card-stats .value { 
  padding-top:15px;
  

}

.card-stats .type { 
  font-size:12px;
  padding-right:5px;
}


.card:hover {
  transform: scale(1.10);
  box-shadow: 5px 5px 15px 5px rgba(0,114,250,0.38);
}
.card {

  transition: 0.5s ease;
  cursor: pointer;
  margin:30px;
}

.button { 
    background-color:rgb(69, 80, 231);
    margin: 0 60px 0 60px;
    padding: 0.5px 0 0.5px 0;
    object-position: center;
    font-size:12px;
    
    
    border-radius: 20px;
    object-fit: center;
}
.button p { 
  font-style:bold;
  color:cornsilk;
}

.button:hover {
  transform: scale(1.05);
  box-shadow: 5px 5px 15px 5px rgba(0,114,250,0.38);
  transition:0.5s ease;
}




</style>