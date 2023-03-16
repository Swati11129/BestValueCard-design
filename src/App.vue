<template>
<v-app>
    <v-container theme="light" style="
    height: 100vh;
    display: grid;
    grid-template-columns: 2fr 1.2fr 1.2fr 2fr;
    grid-template-rows: 1.5fr 4fr 4fr 1.5fr;">
        <v-row theme="light" class="  position color-container">

            <v-col>
                <v-card class="card-position">
                    <div class="ribbon-1 left ">Rotated Ribbon
                    </div>
                </v-card>
            </v-col>
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

}

 

.v-sheet.v-card:not(.v-sheet--outlined) {
    box-shadow: 0px 1px 70px 24px rgba(2, 0, 0, 0.2), 0px 2px 3px 0px rgba(0, 0, 0, -15.86), 0px 1px 5px 0px rgba(0, 0, 0, 0.12);
}

.color-container {
    background-color: #F8FDFD;
}

.ribbon-1 {

    background: #08769b;
    box-shadow: 0 0 0 999px #a3d3e5;
    clip-path: inset(0 -40%);
    color: white
}

.left {
    inset: 0 auto auto 0;
    transform-origin: 100% 0;
    transform: translate(-29.3%) rotate(-45deg);
    background-color: #a3d3e5;
    position: absolute;

    display: flex;
    align-items: center;
    justify-content: center;
    color: white;
    width: 133px;
    height: 48px;
    font-size: larger;
}
</style>
