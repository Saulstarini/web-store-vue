<template >
    <div id="app">
        <h1>{{ title }}</h1>
        <i @click="addProducts" id="addRemoveIcon"><svg xmlns="http://www.w3.org/2000/svg" viewBox="0 0 384 512"><!--! Font Awesome Pro 6.1.1 by @fontawesome - https://fontawesome.com License - https://fontawesome.com/license (Commercial License) Copyright 2022 Fonticons, Inc. --><path d="M352 448H32c-17.69 0-32 14.31-32 32s14.31 31.1 32 31.1h320c17.69 0 32-14.31 32-31.1S369.7 448 352 448zM48 208H160v111.1c0 17.69 14.31 31.1 32 31.1s32-14.31 32-31.1V208h112c17.69 0 32-14.32 32-32.01s-14.31-31.99-32-31.99H224v-112c0-17.69-14.31-32.01-32-32.01S160 14.33 160 32.01v112H48c-17.69 0-32 14.31-32 31.99S30.31 208 48 208z"/></svg></i>
    </div>
    <div v-if="addProducts()" id="options">
        <AddRemoveOptions />
    </div>
</template>

<script>
import AddRemoveOptions from './AddRemoveOptions.vue';

export default {
    name: "HeaderMain",
    props: {
        title: String,
    },
    components: { 
        AddRemoveOptions 
    },
    methods: {
        addProducts() {
        }
    }
}

</script>

<style scoped>

#app {
    padding: 15px;
    padding-bottom: 25px;
    margin: 0 10%;
    max-width: 80%;
    background-color: darkgoldenrod;
    height: 40px;
    text-align: left;
    border-bottom-left-radius: 10px;
    border-bottom-right-radius: 10px;
    display: flex;
    justify-content: space-between;
    vertical-align: middle;
}

h1 {
    color: black;
    font-weight: bolder;
    font-size: x-large;
    margin-top: 10px;
}

#addRemoveIcon {
    height: 20px;
    width: 20px;
    float: right;
    padding: 10px;
}

#options {
    display: none;
}

</style>