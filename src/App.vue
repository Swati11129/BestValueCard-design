<template>
<v-app>
    <v-container theme="light" style="
    height: 100vh;
    display: grid;
    grid-template-columns: 2fr 1.2fr 1.2fr 2fr;
    grid-template-rows: 1.5fr 4fr 4fr 1.5fr;">
        <v-row  class="  position color-container">

           
                <v-card class="card-position ">
                    <!-- <div class="ribbon-1 left  ">BEST VALUE
                    </div> -->
                      <div class="ribbon ribbon-top-left"><span>BEST VALUE</span></div>
                </v-card>
            
        </v-row>
    </v-container>
</v-app>
</template>

<script>
export default {
    name: 'App',

    data: () => ({
        //
    }),
};
</script>

<style>
@import url(https://fonts.googleapis.com/css?family=Lato:700);
.card-position {
    display: flex;
    align-items: center;
    justify-content: center;
    height: 100%
}

.position {
    display: grid; 
    grid-column: 2/span 2;
    grid-row: 2/span 2;
background-color: black;
}

 

.v-sheet.v-card:not(.v-sheet--outlined) {
    box-shadow: 0px 1px 70px 24px rgba(2, 0, 0, 0.2), 0px 2px 3px 0px rgba(0, 0, 0, -15.86), 0px 1px 5px 0px rgba(0, 0, 0, 0.12);
}

.color-container {
    background-color: black;
}


.ribbon {
  width: 150px;
  height: 150px;
  overflow: hidden;
  position: absolute;
}

.box {
  position: relative;
  max-width: 600px;
  width: 90%;
  height: 400px;
  background: #fff;
  box-shadow: 0 0 15px rgba(0,0,0,.1);
}
.ribbon::before,
.ribbon::after {
  position: absolute;
  z-index: -1;
  content: '';
  display: block;
  border: 5px solid #2980b9;
}
.ribbon span {
  position: absolute;
  display: block;
  width: 225px;
  padding: 15px 0;
  background-color: #3498db;
  box-shadow: 0 5px 10px rgba(0,0,0,.1);
  color: #fff;
  font: 700 18px/1 'Lato', sans-serif;
  text-shadow: 0 1px 1px rgba(0,0,0,.2);
  text-transform: uppercase;
  text-align: center;
}


/* top left*/
.ribbon-top-left {
  top: -10px;
  left: -10px;
}
.ribbon-top-left::before,
.ribbon-top-left::after {
  border-top-color: transparent;
  border-left-color: transparent;
}
.ribbon-top-left::before {
  top: 0;
  right: 0;
}
.ribbon-top-left::after {
  bottom: 0;
  left: 0;
}
.ribbon-top-left span {
  right: -25px;
  top: 30px;
  transform: rotate(-45deg);
}


</style>
