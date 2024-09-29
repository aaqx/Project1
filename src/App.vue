
<template>
  <div id="app"> 

    <div class="container">

      <div id="side-bar">
      <Sidebar/>
      </div>
      <div id="main">
      <Header/> 
      </div>
      <div class="date-x d-flex justify-content-start mb-2 ms-3">
      <p><Date/></p>
      </div>

      <div class="filter d-flex justify-content-between">

      <!-- <div class="radio-x">
        <input type="radio" name="radio" >All
        <input type="radio" name="radio">
       </div>

      <div class="input-x">
          <label for="">From</label>
          <input type="date" class="p-2">
          <button class="btn btn-warning text-white">Find</button>
      </div> -->

      </div>


      <div id="stat">

        <div class="cards">

            <div class="col">
              <a href="#"><img src="./assets/img/card-order.svg" alt=""> <span class="opacity-50">Order Number</span> </a>
              <h2 class="text-dark">1000</h2>
              <p class="lead oo">SR</p>
            </div>
          
            <div class="col">
              <a href="#"><img src="./assets/img/card-company.svg" alt=""> <span class="opacity-50">Company Number</span> </a>
              <h2 class="text-dark">1000000</h2>
              <p class="lead oo">SR</p>
            </div>
  
            <div class="col">
              <a href="#"><img src="./assets/img/card-driver.svg" alt=""> <span class="opacity-50">Drivers Number</span> </a>
              <h2 class="text-dark">500</h2>
              <p class="lead oo">Driver</p>
            </div>
  
            <div class="col">
              <a href="#"><img src="./assets/img/card-sales.svg" alt=""> <span class="opacity-50">Total Sales</span> </a>
              <h2 class="text-dark ">500</h2>
              <p class="lead oo">Driver</p>
            </div>

            <div class="col-2">
                <p> Waiting For Loading </p>
              <a href=""><img src="./assets/img/card-load1.svg" alt="" ></a>
            </div>
  
            <div class="col-2">
              <p> Waiting For Arrive </p>
              <a href=""><img src="./assets/img/card-load1.svg" alt="" ></a>
            </div>
  
            <div class="col-2">
              <p> Completed </p>
              <a href=""><img src="./assets/img/card-load1.svg" alt="" ></a>

            </div>

            <div class="col-2">
              <p> Canceled </p>
              <a href=""><img src="./assets/img/card-load1.svg" alt="" ></a>
            </div>

            <div class="col-3 col-3r item1 opacity-100 ps-3">
              <h6> Top 5 Companies </h6>
              <table class="table">
                <thead>
                  <tr >
                    <td> Company Name </td>
                    <td> Order Qty </td>
                    <td> Amount  </td>
                  </tr>
                </thead>
                <tbody>
                  <tr>
                    <td> Gillete </td>
                    <td>5000</td>
                    <td> 50000 SR </td>
                  </tr>
                  <tr>
                    <td> Louis Vuitton </td>
                    <td>3000</td>
                    <td> 50000 SR </td>
                  </tr>
                  <tr>
                    <td> Johnson & Johnson </td>
                    <td>2000</td>
                    <td> 50000 SR </td>
                  </tr>
                  <tr>
                    <td> Nintendo </td>
                    <td>1000</td>
                    <td> 50000 SR </td>
                  </tr>
                </tbody>
              </table>
            </div>

            <div class="col-3">
              <p> Repeated Order </p>
              <a href=""><img src="./assets/img/card-load1-80.svg" alt="" ></a>
            </div>

            <div class="col-3">
              <p> Commission </p>
              <a href=""><img src="./assets/img/card-load2.svg" alt="" ></a>
            </div>

          </div>

      </div>
    </div>
  </div>

</template>

<style>
/* #app{
  border: 2px solid green;
} */
.date-x{
  width: 220px;
}
.oo{
  font-size: x-small;
  flex-direction: row;
  flex-wrap: wrap;
}
.col , .col-2 , .col-3{
border: 1px solid gray;

width: 270px;
border-radius: 5px;
padding-top: 15px;
padding-left: 10px;
font-family: 'Poppins',sans-serif;
font-weight:600;
}
.col-2 , .col-3{
  text-align: center;
  opacity: 100%;
  padding-left: 0%;
  
}
.col-3r{
text-align: start;
}

.col-3{
  grid-row: span 2;
}
.filter button{
margin: 10px;
position: relative;
/* left: 21%; */
}
.filter input{
  position: relative;
/* left: 25%; */
border-radius: 5px;
opacity: 20%;
height: 35px;
border: none;
}

.input-x{
  border: 1px gray solid;
  display: flex;
  justify-content: space-evenly;
  align-items: baseline;

  
}


.item1{
  grid-column: 1/3;
  width: 560px;
}
.cards{
  display: grid;
  grid-template-columns:  repeat(4,270fr);
  grid-template-rows: 120px repeat(2,220px) ;
  gap: 1rem;
  position: absolute;
  margin-left: 10px;

  
}
/*
#stat{
}
*/

.container{
  display: flex;
  /*
  border: 2px solid red;
  */
  width: 1440px;
  height: 1115px;
  margin: 0;
  padding: 0;
  flex-direction: column;
  flex-wrap: wrap;

}
#side-bar{
  background-color: #F6F6F6;
  height: 1115px;
  width: 238px;
}
#side-bar img{
  position: relative;
  left: 15px;
  fill: orange;
  color: aqua;
}
#main{
  width: 1115px;
  height: 50px;
  display: flex;
justify-content: space-between;

}

a{
  color: #353535;
  text-decoration: none;
}


</style>

<!-- import sidebar from './components/sidebar' -->
<script>
import Sidebar from './components/sidebar.vue';
import Header from './components/header.vue';
import Date from './components/date.vue';

export default {
  name:'app',
  components:{
    Header,
    Sidebar,
    Date
  }
};

// function updateDate() {
//             const now = new Date();
//             const options = { 
//                 year: 'numeric', 
//                 month: 'long', 
//                 day: 'numeric', 
//                 hour: '2-digit', 
//                 minute: '2-digit', 
//                 second: '2-digit', 
//                 hour12: false 
//             };
//             document.getElementById('date-x').textContent = now.toLocaleString('en-US', options);
//         }

//         // Update the date every second
//         setInterval(updateDate, 1000);
        
//         // Initial call to display the date immediately
//         updateDate();

</script>


<!-- <template>
  <div id="app">
    <UserProfile name="Jane Doe" bio="Web Developer" />
  </div>
</template>

<script>
import UserProfile from './components/sidebar.vue';

export default {
  name: 'app',
  components: {
    UserProfile
  }
}
</script>

<style>
/* Global styles */
</style>  -->