<template>
    <div id="addRemoveOptions">
        <i @click="addProducts">Add</i>
        <i @click="removeProducts"></i>
        <i @click="closePage">x</i>
    </div>
</template>

<script>
export default {
    name: 'AddRemoveOptions',
    methods: {
        addProducts() {
            console.log('product added')
        },

        removeProducts() {
            console.log('product removed');
        },

        closePage() {
            document.getElementById('addRemoveOptions').style.display = "none";
        }
    }
}
</script>

<style scoped>
#addRemoveOptions {
    height: 25px;
    width: 100px;
    background-color: beige;
    color: black;
    border: 0.5px solid grey;
    float: right;
    margin-right: 13%;
}
</style>