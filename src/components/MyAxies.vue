<template>
    <div class="row justify-content-center">
        <div class="col-9">
            <div class="container d-flex align-items-center justify-content-around border border-4 rounded-pill mt-3">
                <img class="bg-dark rounded-circle my-1" :src="axieImg" alt="axie_pic" width="125" height="120">
                <div class="">
                    <div class="d-flex">
                        <h4 class="fw-bold mt-2 ms-5">{{axieName}}</h4>
                        <h4 class="text-primary fw-bold mt-2 ms-5">{{axieid}}</h4>
                    </div>
                    <a class=" fs-4 fw-bold text-success" :href="axiepage" target="#blank">MySelf FAN page !!!</a>
                </div>
            </div>
        </div>
    </div>
</template>

<script>
export default {
    name: 'MyAxies',
    props: {
        axieName: {
            type: String,
            required: true,
        },
        axieImg: {
            type: String,
            required: true,
        },
        axieid: {
            type: Number,
            required: true,
        },
        axiepage: {
            type: String,
            required: true,
        },
    },
    //   data: function(){
    //       return { }
    //   },
    // computed: {},
    //methods: {}
    // watch: {},
    // components: {},
    // mixins: [],
    // filters: {},
    // -- Lifecycle Methods
    // -- End Lifecycle Methods
}
</script>

<style scoped>

</style>