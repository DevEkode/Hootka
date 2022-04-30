<template>
  <v-container fill-height fluid>
        <v-row align="center" justify="center" style="min-height:50%;">
            Hello
        </v-row>
        <v-row align="center" justify="center" style="min-height:50%;">
            <v-col>
                <v-row align="center" justify="center" class="quiz_btn_block">
                    <v-btn block height="100%">
                        <v-icon>mdi-cards-heart</v-icon>
                    </v-btn>
                </v-row>
                <v-row align="center" justify="center" class="quiz_btn_block">
                    <v-btn block height="100%">
                        <v-icon>mdi-cards-spade</v-icon>
                    </v-btn>
                </v-row>
            </v-col>
            <v-col>
                <v-row align="center" justify="center" class="quiz_btn_block">
                    <v-btn block height="100%">
                        <v-icon>mdi-cards-club</v-icon>
                    </v-btn>
                </v-row>
                <v-row align="center" justify="center" class="quiz_btn_block">
                    <v-btn block height="100%">
                        <v-icon>mdi-cards-diamond</v-icon>
                    </v-btn>
                </v-row>
            </v-col>
        </v-row>
    </v-container>
</template>

<script lang="ts">
import Vue from 'vue'
export default Vue.extend({
    
})
</script>

<style>
    .quiz_btn_block {
        height:20vh;
        padding:1%;
    }
</style>