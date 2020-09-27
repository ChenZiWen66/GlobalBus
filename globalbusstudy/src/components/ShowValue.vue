<template>
    <div>
        <p id="passage">这是一段话</p>
    </div>
</template>

<script>
    import {globalBus} from "./GlobalBus";

    export default {
        name: "ShowValue",
        mounted() {
            this.changeValue();
        },
        methods:{
            changeValue(){
                globalBus.$on('message_fromPassageComponent',function (message) {
                    console.log("aaaaaaaaaa");
                    $("#passage").text(message);
                })
            }
        }
    }
</script>

<style scoped>

</style>