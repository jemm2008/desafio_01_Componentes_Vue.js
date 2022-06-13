<template>
    <div id="app" class="container">
        <!--<img alt="Vue logo" src="./assets/logo.png">
        <HelloWorld msg="Welcome to Your Vue.js App"/> -->
        <h1 class="bg-info rounded-pill mx-5"> Nuevo Componente: <span class="fw-bold">{{title}}</span></h1>
        <MyAxies v-for="axie in axies" :key="axie.id"
            :axieName="axie.nombre"
            :axieImg="axie.src"
            :axieid= "axie.id"
            :axiepage= "axie.page"
        />
    </div>
</template>

<script>
    // import HelloWorld from './components/HelloWorld.vue'
    import MyAxies from '@/components/MyAxies.vue'


    export default {
        name: 'App',
        data(){
            return {
                title: "My Axies",
                axies: [
                    {
                        id: 3179575,
                        nombre: "Faster Fish!!",
                        src: "https://axiecdn.axieinfinity.com/axies/3179575/axie/axie-full-transparent.png",
                        page: "https://marketplace.axieinfinity.com/axie/3179575/"
                    },
                    {
                        id: 2479271,
                        nombre: "Pollito PIO_!!",
                        src: "https://axiecdn.axieinfinity.com/axies/2479271/axie/axie-full-transparent.png",
                        page: "https://marketplace.axieinfinity.com/axie/2479271/"
                    },
                    {
                        id: 2278510,
                        nombre: "Jack Sparrow_!!",
                        src: "https://axiecdn.axieinfinity.com/axies/2278510/axie/axie-full-transparent.png",
                        page: "https://marketplace.axieinfinity.com/axie/2278510/"
                    },
                    {
                        id: 1962478,
                        nombre: "Hércules VG01",
                        src: "https://axiecdn.axieinfinity.com/axies/1962478/axie/axie-full-transparent.png",
                        page: "https://marketplace.axieinfinity.com/axie/1962478/"
                    },
                    {
                        id: 8641768,
                        nombre: "virgin scaly",
                        src: "https://axiecdn.axieinfinity.com/axies/8641768/axie/axie-full-transparent.png",
                        page: "https://marketplace.axieinfinity.com/axie/8641768/"
                    },
                    {
                        id: 1409689,
                        nombre: "DapiDOX_!! Jr. VG3",
                        src: "https://axiecdn.axieinfinity.com/axies/1409689/axie/axie-full-transparent.png",
                        page: "https://marketplace.axieinfinity.com/axie/1409689/"
                    },     
                    {
                        id: 10874427,
                        nombre: "BestBird",
                        src: "https://axiecdn.axieinfinity.com/axies/10874427/axie/axie-full-transparent.png",
                        page: "https://marketplace.axieinfinity.com/axie/10874427/"
                    }
                ]
            }
        },
        components: {
            // HelloWorld,
            MyAxies
        }
    }
</script>

<style>
    #app {
        font-family: Avenir, Helvetica, Arial, sans-serif;
        -webkit-font-smoothing: antialiased;
        -moz-osx-font-smoothing: grayscale;
        text-align: center;
        color: #2c3e50;
        margin-top: 60px;
    }
    body {
        background-image: url('@/assets/imagenfondo.png'); 
    }
    span {
        color: red;
    }
</style>
