<template>
    <b-col cols="6" class="padding">
        <div class="text-center">
            <i v-bind:class="app.icon"></i>
            <h5>{{app.name}}</h5>
        </div>
    </b-col>
</template>

<script>
export default {
    name: 'App',
    props: {
        app: Object
    }
}
</script>

<style scoped>
    * {
        color: rgba(255, 255, 255, .75);
    }

    h5 {
        padding-top: 5px; 
    }
    .icons {
        font-size: 50px!important;
        color: rgba(255, 255, 255, .75)
    }
    .padding {
        padding: 20px 0;
    }

</style>