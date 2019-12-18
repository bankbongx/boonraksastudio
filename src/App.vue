<template>
    <v-app>
        <v-app-bar app color="blue-grey" dark>
            <div class="d-flex align-center">
                <v-img alt="Boonraksa Logo" class="shrink mr-2" contain src="./assets/logos.png" transition="scale-transition" width="40" />
                <h3 class="font-weight-thin change-font">บุญรักษา สตูดิโอ</h3>
            </div>
    
            <v-spacer></v-spacer>
    
            <v-btn href="https://www.facebook.com/boonruksastudio" target="_blank" text>
                <span class="mr-2 change-font">ติดต่อเรา</span>
                <v-icon>mdi-facebook</v-icon>
            </v-btn>
        </v-app-bar>
    
        <v-content>
            <Content/>
        </v-content>
    </v-app>
</template>

<script>
import Content from './components/Content';

export default {
    name: 'App',

    components: {
        Content,
    },

    data: () => ({
        //
    }),
};
</script>
<style>
.change-font {
font-family: 'Sarabun', sans-serif;
}
.v-application a {
    color: white;
}
</style>