<template>
  <v-container fill-height fluid>
        <v-row align="center" justify="center" style="min-height:40%;">
            <v-col>
                <v-row align="center" justify="center"> 
                    <h1 class="text-center">Combien font 1+1 ?</h1>
                </v-row>
            </v-col>
        </v-row>
        <v-row style="min-height:60%;">
            <v-col cols="12">
                <v-row align="center" justify="center"> 
                    <h3 class="text-center font-weight-light d-block d-sm-none">Regarde le tableau pour voir les propositions</h3>
                </v-row>
            </v-col>
            <v-col cols="6">
                <v-row align="center" justify="center" class="quiz_btn_block">
                    <v-btn block height="150" class="red darken-4 quiz-btn">
                        <v-icon>mdi-cards-heart</v-icon>
                        <span class="ml-2 d-none d-sm-block">2</span>
                    </v-btn>
                </v-row>
                <v-row align="center" justify="center" class="quiz_btn_block">
                    <v-btn block height="150" class="orange darken-4 quiz-btn">
                        <v-icon>mdi-cards-spade</v-icon>
                        <span class="ml-2 d-none d-sm-block">Le portugal</span>
                    </v-btn>
                </v-row>
            </v-col>
            <v-col cols="6">
                <v-row align="center" justify="center" class="quiz_btn_block">
                    <v-btn block height="150" class="blue darken-4 quiz-btn">
                        <v-icon>mdi-cards-club</v-icon>
                        <span class="ml-2 d-none d-sm-block">π/2</span>
                    </v-btn>
                </v-row>
                <v-row align="center" justify="center" class="quiz_btn_block">
                    <v-btn block height="150" class="green darken-4 quiz-btn">
                        <v-icon>mdi-cards-diamond</v-icon>
                        <span class="ml-2 d-none d-sm-block">La réponse D</span>
                    </v-btn>
                </v-row>
            </v-col>
        </v-row>
    </v-container>
</template>

<script lang="ts">
import Vue from 'vue'
export default Vue.extend({
    computed: {

    }
})
</script>

<style>
    .quiz_btn_block {
        padding:1%;
    }

    .quiz-btn {
        font-size: 1.5em !important;
        text-transform:none !important;
    }
</style>