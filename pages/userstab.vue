<template>
    <div class="home">
       
   <h5>Users</h5>

    </div>
</template>

<script setup>

import { ref } from 'vue';/* 
import { countries } from 'country-list-json';  */
import { languagesAll, countries } from 'countries-list';

definePageMeta({
    layout: 'nav'
})
const isVisible = ref(false)

const open_approval = () => {
    isVisible.value = !isVisible.value
}


</script>


<style scoped>
.home {
    background: white;
    height: 100vh;
    overflow: auto;
    overflow: -moz-scrollbars-none;
    -ms-overflow-style: none;
    scrollbar-width: none;
    margin: 0px;
    padding: 0px;
    -ms-overflow-style: none !important;
    /* for Internet Explorer, Edge */
    width: 100%;
}

.home_page {
    background: whitesmoke;
    height: 100vh;
    overflow: auto;
    overflow: -moz-scrollbars-none;
    -ms-overflow-style: none;
    scrollbar-width: none;
    margin: 0px;
    padding: 0px;
    -ms-overflow-style: none !important;
    /* for Internet Explorer, Edge */
    width: 100%;
}

.main_form {
    width: 80%;
    margin: auto;
    margin-top: 5rem;
}

.main_form h5,
.main_form p {
    text-align: center;
}

.formgroup input:focus,
.formgroup select:focus,
.formgroup textarea:focus {
    box-shadow: none;
    outline: none;
}

.formgroup button {
    display: block;
    width: 50%;
    margin: auto;
    color: white;
    background: #FB0A03;
    ;
}
</style>