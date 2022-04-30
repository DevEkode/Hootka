<template>
    <v-container fill-height fluid>
        <v-row align="center"
            justify="center">
            <v-col cols="0" md="2" lg="4"></v-col>
            <v-col cols="12" md="8" lg="4">
                <v-card elevation="2">
                    <v-card-title primary-title>
                        Login
                    </v-card-title>
                    <v-card-text>
                        <v-text-field
                            name="username"
                            label="Username"
                            id="username"
                            prepend-icon="mdi-account"
                            outlined
                        ></v-text-field>
                        <v-text-field
                            name="password"
                            label="Password"
                            id="password"
                            prepend-icon="mdi-lock"
                            :append-icon="hidePassword ? 'mdi-eye-off' : 'mdi-eye'"
                            @click:append="tooglePassShow"
                            outlined
                            :type="hidePassword ? 'password' : 'text'"
                        ></v-text-field>
                        <v-btn color="primary">Login</v-btn>
                    </v-card-text>
                </v-card>
            </v-col>
            <v-col cols="0" md="2" lg="4"></v-col>
        </v-row>
    </v-container>
</template>

<script lang="ts">
import Vue from 'vue'
export default Vue.extend({
    data() {
        return {
            hidePassword: true
        }
    },
    methods: {
        tooglePassShow() {
            this.hidePassword = !this.hidePassword;
        }
    }
})
</script>

<style>

</style>