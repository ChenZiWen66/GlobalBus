<template>
    <div>
        <p @click="sentMessage('A')">段落A</p>
        <p @click="sentMessage('B')">段落B</p>
        <p @click="sentMessage('C')">段落C</p>
    </div>
</template>

<script>
    import {globalBus} from "./GlobalBus";

    export default {
        name: "PassageComponent",
        methods:{
            sentMessage(message){
                globalBus.$emit('message_fromPassageComponent',[message,'aaaaaa']);
            }
        }
    }
</script>

<style scoped>

</style>