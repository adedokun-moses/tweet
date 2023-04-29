<template>
    <main>
        <div class="tab_section">
            <ul class="nav nav-tabs mb-3" id="ex1" role="tablist">
                <li class="nav-item" role="presentation">
                    <a class="nav-link active" id="ex1-tab-1" data-bs-toggle="tab" href="#ex1-tabs-1" role="tab"
                        aria-controls="ex1-tabs-1" aria-selected="true">All Movies</a>
                </li>
                <li class="nav-item" role="presentation" style="margin-left: 10rem;">
                    <a class="nav-link" id="ex1-tab-2" data-bs-toggle="tab" href="#ex1-tabs-2" role="tab"
                        aria-controls="ex1-tabs-2" aria-selected="false">Produces Movies</a>
                </li>
                <li class="nav-item" role="presentation"  style="margin-left: 10rem;">
                    <a class="nav-link" id="ex1-tab-3" data-bs-toggle="tab" href="#ex1-tabs-3" role="tab"
                        aria-controls="ex1-tabs-3" aria-selected="false">Purchased Movies</a>
                </li>
            </ul>
            <div class="tab-content" id="ex1-content">
                <div class="tab-pane fade show active" id="ex1-tabs-1" role="tabpanel" aria-labelledby="ex1-tab-1">
                     <div class="row">
                        <div class="col-sm-4 ">
                           <div class="row">
                            <div class="col-sm-11 movie_display mx-auto">
                                <div class="image_tab">
                                    <div>
                                        <img src="../assets/pana.png"  alt="">
                                    </div>
                                    <div>
                                        <h3> <i class="fa fa-edit"><span class="mr-5">Edit</span></i> </h3>
                                        <h3><i class="fa fa-trash "><span class="mr-5">Delete</span></i></h3>
                                    </div>
                                </div>

                            </div>
                           </div>
                        </div>
                        <div class="col-sm-4 ">
                           <div class="row">
                            <div class="col-sm-11 movie_display mx-auto">

                            </div>
                           </div>
                        </div>
                        <div class="col-sm-4 ">
                           <div class="row">
                            <div class="col-sm-11 movie_display mx-auto">

                            </div>
                           </div>
                        </div>
                     </div>
                </div>
                <div class="tab-pane fade" id="ex1-tabs-2" role="tabpanel" aria-labelledby="ex1-tab-2">
                    Tab 2 content
                </div>
                <div class="tab-pane fade" id="ex1-tabs-3" role="tabpanel" aria-labelledby="ex1-tab-3">
                    Tab 3 content
                </div>
            </div>
        </div>


    </main>
</template>

<script  setup>

definePageMeta({
    layout: 'nav'
})

</script>


<style scoped>
main {
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

.tab_section{
    width: 90%;
    margin: 3rem auto 0px auto;
}

.nav-tabs {
    border: none !important;
    background: #F7F8FA;
    padding: 10px 0px 0px 0px;
}
.nav-item{
    border: none !important;
    outline: none !important;
} 
.nav-item a{
    color: black;
    font-size: 15px;
    font-weight: 500;
}
.nav-link a:active{
    color: red;
} 

.movie_display {
    height: 150px;
    background: whitesmoke;
    border-radius: 1px;
}

.image_tab{
    height: 120px;
    overflow: hidden;
    margin: 10px;
    display: flex;
    align-items: center;
}

.image_tab img{
    width: 60%;
}

.image_tab h3{
    font-size: 10px;
}
</style>