<template>
<v-app style="background-color:#E8E8E8;">
    <v-container >
            <v-card :elevation="2" class="card-position position " >
                <div class="ribbon ribbon-top-left"><span>BEST VALUE</span></div>
            </v-card>
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

/*
.position {
    display: flex;
    align-items: center;
    justify-content: center;
    height: 80%
}
*/
.ribbon {
    width: 150px;
    height: 150px;
    overflow: hidden;
    position: absolute;
}
.ribbon span {
    position: absolute;
    display: block;
    width: 225px;
    padding: 15px 0;
    background-color: #6FC2EE;
    box-shadow: 0 5px 10px rgba(0, 0, 0, .1);
    color: #fff;
    font: 700 18px/1 'Lato', sans-serif;
    text-shadow: 0 1px 1px rgba(111, 194, 238, .2);
    text-transform: uppercase;
    text-align: center;
}

.ribbon-top-left {
    top: -10px;
    left: -10px;
}
.ribbon-top-left span {
    right: -25px;
    top: 30px;
    transform: rotate(-45deg);
}
</style>
