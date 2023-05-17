<template>
    <div class="home">

        <form class="main_form">
            <h5>Users Form </h5>
            <p>Ensure all details are filled correctly </p>

            <div class="formgroup mt-5">
                <div class="row">
                    <div class="col-6 ">
                        <label> First Name </label>
                        <input type="text" placeholder="First Name" class="form-control mt-2">
                    </div>
                    <div class="col-6 ">
                        <label> Last Name </label>
                        <input type="text" placeholder="Last Name" class="form-control mt-2">
                    </div>
                </div>
            </div>
            <div class="formgroup mt-4">
                <div class="row">
                    <div class="col-6 ">
                        <label>Language</label>
                        <select class="form-control mt-2">
                            <option v-for="lang in languagesAll" :key="lang.name">{{ lang.name }}</option>
                        </select>

                    </div>
                    <div class="col-6 ">
                        <label>Genre</label>
                        <select class="form-control mt-2">
                            <option>Genre</option>
                            <option>Spanish</option>
                            <option>French</option>
                        </select>

                    </div>
                </div>

            </div>
            <div class="formgroup mt-4">
                <div class="row">
                    <div class="col-6 ">
                        <label>Wood</label>
                        <select class="form-control mt-2">
                            <option>Nollywood</option>
                            <option>Bollywood</option>
                        </select>

                    </div>
                    <div class="col-6 ">
                        <label>Type</label>
                        <select class="form-control mt-2">
                            <option>Spanish</option>
                            <option>French</option>
                        </select>

                    </div>
                </div>

            </div>
            <div class="formgroup mt-4">
                <div class="row">
                    <div class="col-6 ">

                        <label>Rating</label>
                        <select class="form-control mt-2">
                            <option>1</option>
                            <option>2</option>
                            <option>3</option>
                        </select>

                    </div>
                    <div class="col-6 ">
                        <label>Movie Orginal Language</label>
                        <select class="form-control mt-2">
                            <option v-for="lang in languagesAll" :key="lang.name">{{ lang.name }}</option>
                        </select>

                    </div>
                </div>

            </div>

            <div class="formgroup mt-4">
                <label>Symposis</label>
                <input type="text" placeholder="Symposis" class="form-control mt-2">
            </div>
   

            <div class="formgroup mt-4">
                <label style="font-weight: 500;">Movie Type</label>
                <ul class="nav nav-tabs nav-fill mb-3 mt-3" id="ex1" role="tablist">
                    <li class="nav-item" role="presentation">
                        <a class="nav-link active" id="ex2-tab-1" data-bs-toggle="tab" href="#ex2-tabs-1" role="tab"
                            aria-controls="ex2-tabs-1" aria-selected="true">Single Movie</a>
                    </li>
                    <li class="nav-item" role="presentation">
                        <a class="nav-link" id="ex2-tab-2" data-bs-toggle="tab" href="#ex2-tabs-2" role="tab"
                            aria-controls="ex2-tabs-2" aria-selected="false">Multi Movie</a>
                    </li>
                    <li class="nav-item" role="presentation">
                        <a class="nav-link" id="ex2-tab-3" data-bs-toggle="tab" href="#ex2-tabs-3" role="tab"
                            aria-controls="ex2-tabs-3" aria-selected="false">Series Movie</a>
                    </li>
                </ul>
                <div class="tab-content" id="ex2-content">
                    <div class="tab-pane fade show active" id="ex2-tabs-1" role="tabpanel" aria-labelledby="ex2-tab-1">
                        <input type="text" placeholder="Duration" class="form-control">
                    </div>
                    <div class="tab-pane fade" id="ex2-tabs-2" role="tabpanel" aria-labelledby="ex2-tab-2">
                        <div class="row">
                            <div class="col-6">
                                <input type="text" placeholder="Number Of Parts" class="form-control">
                            </div>
                            <div class="col-6">
                                <input type="text" placeholder="Duration" class="form-control">
                            </div>
                        </div>
                    </div>
                    <div class="tab-pane fade" id="ex2-tabs-3" role="tabpanel" aria-labelledby="ex2-tab-3">
                        <div class="row">
                            <div class="col-4">
                                <input type="text" placeholder="Number Of Seasons" class="form-control">
                            </div>
                            <div class="col-4">
                                <input type="text" placeholder="Season 1 Episodes" class="form-control">
                            </div>
                            <div class="col-4">
                                <input type="text" placeholder="Duration (total) S1E1:" class="form-control">
                            </div>
                        </div>
                    </div>
                </div>

            </div>
            <div class="formgroup mt-4">
                <div class="row">
                    <div class="col-4">
                        <label>Year Produced</label>
                        <input type="text" placeholder="Year Produced" class="form-control mt-3">

                    </div>
                    <div class="col-4">
                        <label>Executive Producer</label>
                        <select class="form-control mt-3">
                            <option>Executive Producer</option>
                            <option>Spanish</option>
                            <option>French</option>
                        </select>

                    </div>
                    <div class="col-4">
                        <label>Production Company</label>
                        <select class="form-control mt-3">
                            <option>Production Company</option>
                            <option>Spanish</option>
                            <option>French</option>
                        </select>

                    </div>
                </div>

            </div>

            <div class="formgroup mt-4">
                <div class="row">
                    <div class="col-4">
                        <label>Script Original language</label>
                        <select class="form-control mt-3">
                            <option v-for="lang in languagesAll" :key="lang.name">{{ lang.name }}</option>
                        </select>

                    </div>
                    <div class="col-4">
                        <label>Script written by</label>
                        <select class="form-control mt-3">
                            <option>Executive Producer</option>
                            <option>Spanish</option>
                            <option>French</option>
                        </select>

                    </div>
                    <div class="col-4">
                        <label>Script Original Language Location</label>
                        <select class="form-control mt-3">
                            <option v-for="country in countries" :key="country.name">{{ country.name }}</option>
                        </select>

                    </div>
                </div>

            </div>

            <div class="formgroup mt-4">
                <div class="row">
                    <div class="col-4">
                        <label>Script Translated Language</label>
                        <select class="form-control mt-3">
                            <option v-for="lang in languagesAll" :key="lang.name">{{ lang.name }}</option>
                        </select>

                    </div>
                    <div class="col-4">
                        <label>Script Translated By</label>
                        <select class="form-control mt-3">
                            <option>Executive Producer</option>
                            <option>Spanish</option>
                            <option>French</option>
                        </select>

                    </div>
                    <div class="col-4">
                        <label>Script Translated Language Location</label>
                        <select class="form-control mt-3">
                           <option v-for="country in countries" :key="country.name">{{ country.name }}</option>
                          
                        </select>

                    </div>
                </div>

            </div>


            <div class="formgroup mt-4">
                <button class="btn">Submit</button>
            </div>



        </form>



    </div>
</template>

<script  setup>

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