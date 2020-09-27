<template>
    <div>
        <PassageComponent/>
        <ShowValue/>
    </div>
</template>

<script>
    import PassageComponent from "../components/PassageComponent";
    import ShowValue from "../components/ShowValue";

    export default {
        name: "TestPage",
        components:{
            PassageComponent,ShowValue
        }
    }
</script>

<style scoped>

</style>