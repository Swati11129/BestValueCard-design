<template>
<v-app style="background-color:#E8E8E8;">
    <v-container >
            <v-card :elevation="2" class="card-position position rounded-xl " >
                <!-- <div class="ribbon ribbon-top-left"><span>BEST VALUE</span></div> -->
                <div class="stack-top left" style="--d:12px;--w:200px; --c:skyblue;">BEST VALUE</div>
            </v-card>
    </v-container>
</v-app>
</template>

<script>

export default {
    name: 'BestValueCard',

    data: () => ({
        //
    }),
};
</script>

<style>
@import url(https://fonts.googleapis.com/css?family=Lato:700);
.container {
    height: 100vh;
    display: grid;
    grid-template-columns: 2fr 1.2fr 1.2fr 2fr;
    grid-template-rows: 1.5fr 4fr 4fr 1.5fr;
    margin:auto;
    
}

.card-position {
    grid-column: 2/span 2;
    grid-row: 2/span 2;
    height:100%;
    width: 100%;
    background-color:#FEFEFE;

}

.stack-top {
  /* adjust the below to control the shape */
  --d:5px; 
  --w:100px;
  --c:skyblue;
  /**/

  position: absolute;
  top: 0;
  right: 0;
  transform: translate(29.29%, -100%) rotate(45deg); /* 29.29% = 100%*(1 - cos(45deg)) */
  color: #fff;
  text-align: center;
  width: var(--w);
  transform-origin: bottom left;
  padding:5px 0 calc(var(--d) + 5px);
  background:
    linear-gradient(rgba(0,0,0,0.6) 0 0) bottom/100% var(--d) no-repeat
    var(--c);
    font-family: 'Poppins',sans-serif;
    font-weight: 550;
  clip-path:polygon(0 100%,0 calc(100% - var(--d)),50% calc(100% - var(--d) - var(--w)/2),100% calc(100% - var(--d)),100% 100%,calc(100% - var(--d)) calc(100% - var(--d)), var(--d) calc(100% - var(--d)))
}

.stack-top.left {
  left:0;
  right:auto;
  transform: translate(-29.29%, -100%) rotate(-45deg);
  transform-origin: bottom right;
}

</style>
