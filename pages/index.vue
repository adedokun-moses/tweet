<template>
    <div class="container-fluid m-0 p-0">


        <div :class="[isActive ? 'home' : 'home_page']">
            <div class="row">
                <div class="col-sm-11 mx-auto ">
                    <div class="row">
                        <div class="col-sm-12 pt-3">
                            <div class="row">
                                <div class="col-sm-8 m-0 p-0">
                                    <h5>Hey, Bistom</h5>
                                    <p>Here’s what is happening in your workspace</p>
                                </div>
                                <div class="col-sm-4 d-flex m-0 p-0 ">
                                    <div class="search_btn">
                                        <input type="text" placeholder="Search " id="">
                                    </div>

                                    <div class="toggleBn ">
                                        <input type="checkbox" @click="toggleDarkMode" class="checkbox" id="checkbox">
                                        <label for="checkbox" class="checkbox-label">
                                            <i class="fas fa-moon"></i>
                                            <i class="fas fa-sun"></i>
                                            <span class="ball"></span>
                                        </label>
                                    </div>
                                </div>
                            </div>

                        </div>
                        <div class="col-sm-12 action_tab mt-4">
                            <h5>Action</h5>
                            <div class="view_tab d-flex">
                                <div>
                                    <h5>Create View</h5>
                                </div>
                                <div class="shift">
                                    <h5><i class="fa fa-message"></i> New Feedback</h5>
                                </div>
                                <div>
                                    <h5><i class="fa-solid fa-leaf"></i> New Initiative</h5>
                                </div>
                                <div>
                                    <h5><i class="fa-solid fa-pizza-slice"></i> New design task</h5>
                                </div>
                                <div>
                                    <h5><i class="fa fa-bug"></i> New Bug</h5>
                                </div>
                            </div>
                        </div>

                        <div class="col-sm-12 starred_board mt-5">
                            <h5>Starred Boards <span><i class="fa fa-plus" style="float: right;"></i></span></h5>
                            <div class="row">
                                <div class="col-sm-10 design_plat m-0 p-0 mt-3">

                                    <div class=" design_tab ">
                                        <h5><img src="../assets/blossom.png" alt=""> Front-end <span
                                                style="color:  #989898;"><br> The cool guys board</span></h5>
                                        <img src="../assets/f.png" alt="" class="mt-5" style="margin-left: 15px;">
                                    </div>
                                    <div class=" design_tab ">
                                        <h5><img src="../assets/a.png" alt=""> Design <span style="color:  #989898;"><br>
                                                The cool guys board</span></h5>
                                        <img src="../assets/ff.png" alt="" class="mt-5" style="margin-left: 15px;">
                                    </div>
                                    <div class=" design_tab ">
                                        <h5><img src="../assets/m.png" alt=""> Road-map <span style="color:  #989898; "><br>
                                                The cool guys board</span></h5>
                                        <img src="../assets/fff.png" alt="" class="mt-5" style="margin-left: 15px;">
                                    </div>


                                </div>
                            </div>

                        </div>

                        <div class="col-sm-12 team_tab mt-4">
                            <h5 class="mt-3">Your Team</h5>
                            <div class="row">
                                <div class="team_member d-flex ">

                                    <div class="team col-sm-1">
                                        <i class="fa fa-plus"></i>
                                        <h4>Invite new <br> member</h4>
                                    </div>

                                    <div class="team col-sm-1">
                                        <img src="../assets/em.png" alt="">
                                        <h5><span style="font-weight: bold;">Ekene</span> <br> <span
                                                style="color: #989898; font-size: 10px;">Viewing Bugs</span> </h5>
                                    </div>
                                    <div class="team col-sm-1">
                                        <img src="../assets/g1.png" alt="">
                                        <h5><span style="font-weight: bold;">Daniel</span> <br> <span
                                                style="color: #989898; font-size: 10px;">Offline</span> </h5>
                                    </div>
                                    <div class="team col-sm-1">
                                        <img src="../assets/g2.png" alt="">
                                        <h5><span style="font-weight: bold;">Gift</span> <br> <span
                                                style="color: #989898; font-size: 10px;">Viewing Inbox</span> </h5>
                                    </div>
                                    <div class="team col-sm-1">
                                        <img src="../assets/g3.png" alt="">
                                        <h5><span style="font-weight: bold;">Toluene</span> <br> <span
                                                style="color: #989898; font-size: 10px;">Offline</span> </h5>
                                    </div>
                                    <div class="team col-sm-1">
                                        <img src="../assets/g4.png" alt="">
                                        <h5><span style="font-weight: bold;">Ayo</span> <br> <span
                                                style="color: #989898; font-size: 10px;">Viewing Bugs</span> </h5>
                                    </div>
                                    <div class="team col-sm-1">

                                        <img src="../assets/g4.png" alt="">
                                        <h5><span style="font-weight: bold;">Temi</span> <br> <span
                                                style="color: #989898; font-size: 10px;">Not Signed In</span> </h5>
                                    </div>
                                    <div class="team col-sm-1">
                                        <img src="../assets/g2.png" alt="">
                                        <h5><span style="font-weight: bold;">Gift</span> <br> <span
                                                style="color: #989898; font-size: 10px;">Viewing Inbox</span> </h5>
                                    </div>
                                    <div class="team col-sm-1">
                                        <img src="../assets/g3.png" alt="">
                                        <h5><span style="font-weight: bold;">Toluene</span> <br> <span
                                                style="color: #989898; font-size: 10px;">Offline</span> </h5>
                                    </div>
                                    <div class="team col-sm-1">
                                        <img src="../assets/g4.png" alt="">
                                        <h5><span style="font-weight: bold;">Ayo</span> <br> <span
                                                style="color: #989898; font-size: 10px;">Viewing Bugs</span> </h5>
                                    </div>

                                </div>
                            </div>
                        </div>

                        <div class="col-sm-12 tab_mode">
                            <h5>Recently Created</h5>
                            <h5 class="h5_format">All Assigneess <i class="fa fa-caret-down"></i></h5>
                            <h5 class="h5_format"><i class="fa fa-eye-slash"></i> 6 hidden properties <i
                                    class="fa fa-caret-down"></i></h5>

                            <div class="row">
                                <div class="create_tab col-sm-12">
                                    <div class="row">
                                        <div class="col-sm-8 display_design">
                                            <div class="food_class">
                                                <h3><i class="fa-solid fa-pizza-slice mr-2"></i> CYC-82</h3>
                                            </div>
                                            <div>
                                                <h3 style="font-size: 17px; font-weight: bold
                                                                        ;">Improve dark mode</h3>
                                            </div>

                                        </div>
                                        <div class="col-sm-4 font_design">
                                            <h3>Design</h3>
                                            <i class="fa fa-message"></i>
                                            <i class="fa fa-crown"></i>
                                            <i class="fa fa-user"></i>
                                            <i class="fas fa-user-circle"></i>
                                        </div>
                                    </div>
                                </div>

                                <div class="create_tab col-sm-12 mt-3">
                                    <div class="row">
                                        <div class="col-sm-8 display_design">
                                            <div class="food_class">
                                                <h3><i class="fa-solid fa-leaf mr-2" style="color: green;"></i> CYC-81</h3>
                                            </div>
                                            <div>
                                                <h3 style="font-size: 17px; font-weight: bold
                                                                        ;">Improve dark mode</h3>
                                            </div>

                                        </div>
                                        <div class="col-sm-4 font_design">
                                            <h3 style="background: #FCEAD2;">Front</h3>
                                            <i class="fa fa-message"></i>
                                            <i class="fa fa-crown"></i>
                                            <i class="fa fa-user"></i>
                                            <i class="fas fa-user-circle"></i>
                                        </div>
                                    </div>
                                </div>
                                <div class="create_tab col-sm-12 mt-3">
                                    <div class="row">
                                        <div class="col-sm-8 display_design">
                                            <div class="food_class">
                                                <h3><i class="fa-solid fa-mobile mr-2" style="color: black;"></i> CYC-80
                                                </h3>
                                            </div>
                                            <div>
                                                <h3 style="font-size: 17px; font-weight: bold
                                                                        ;">Improve dark mode</h3>
                                            </div>

                                        </div>
                                        <div class="col-sm-4 font_design">
                                            <h3>Mobile</h3>
                                            <i class="fa fa-message"></i>
                                            <i class="fa fa-crown"></i>
                                            <i class="fa fa-user"></i>
                                            <i class="fas fa-user-circle"></i>
                                        </div>
                                    </div>
                                </div>
                                <div class="create_tab col-sm-12 mt-3">
                                    <div class="row">
                                        <div class="col-sm-8 display_design">
                                            <div class="food_class">
                                                <h3><i class="fa-solid fa-laptop mr-2"></i> CYC-78</h3>
                                            </div>
                                            <div>
                                                <h3 style="font-size: 17px; font-weight: bold
                                                    ;">Improve dark mode</h3>
                                            </div>

                                        </div>
                                        <div class="col-sm-4 font_design">
                                            <h3 style="background: #FBEBF5;">Product</h3>
                                            <i class="fa fa-message"></i>
                                            <i class="fa fa-crown"></i>
                                            <i class="fa fa-user"></i>
                                            <i class="fas fa-user-circle"></i>
                                        </div>
                                    </div>
                                </div>
                            </div>
                        </div>

                    </div>
                </div>
            </div>
        </div>
    </div>
</template>

<script >
import { ref } from 'vue';

export default {
    setup() {
        const isActive = ref(false);

        function toggleDarkMode() {
            //  home.value = !home.value;

            if (isActive.value) {
                isActive.value = false;
            } else {
                isActive.value = true;
            }
        }

        return { isActive, toggleDarkMode };
    },
};


</script>


<style scoped>
.home {
    background: #BCB7B7;
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


.home::-webkit-scrollbar {
    display: none;
}
.home_page::-webkit-scrollbar {
    display: none;
}

.search_btn input {
    background: #EDEDED;
    margin-top: 20px;
    padding: 9px;
    border-radius: 8px;
    width: 100%;
    border: none;
}

.search_btn input:focus {
    background: #EDEDED;
    border-radius: 8px;
    width: 100%;
    border: none;
    outline: none;
}

.action_tab {
    background: #FFFFFF;
    box-shadow: 0px 0px 20px rgba(0, 0, 0, 0.08);
    border-radius: 8px;
    height: 105px;
}

.action_tab h5 {
    font-size: 16px;
    font-weight: bold;
    margin: 7px 0px;
}

.view_tab>div {
    margin: 10px 10px;
    color: #509994;
    background: #F1FBFC;
    border-radius: 8px;

}

.view_tab h5 {
    font-size: 10px;
    padding: 8px 10px;
}

.starred_board h5 {
    font-weight: bold;
}

.design_plat {
    justify-content: space-between;
    display: flex;
}

.design_plat>div {
    margin: 0px;
    padding: 0px;
    width: 270px;
    height: 130px;
    background: #FFFFFF;
    box-shadow: 0px 0px 20px rgba(0, 0, 0, 0.08);
    border-radius: 12px;
}

.design_tab h5 {
    font-size: 13px;
    margin: 15px 0px 0px 15px;
}

.team_tab {
    height: 200px;
    background: #FFFFFF;
    box-shadow: 0px 0px 20px rgba(0, 0, 0, 0.08);
    border-radius: 12px;
}

.team_tab h5 {
    font-weight: bold;
}

.team_member {
    align-items: center;
    overflow: auto;
    scrollbar-width: none;

}

.team_member::-webkit-scrollbar {
    display: none;
}

.team_member scrollbar-width {
    display: none;

}

.team_member>div {
    margin: 20px;
}

.team h4 {
    font-size: 14px;
    text-align: center;
    color: #BCB7B7;
    padding-top: 10px;
}

.team i {
    padding: 2em;
    background: #BCB7B7;
    border-radius: 40px;
    margin-left: 8px;
}

.team img {
    display: block;
    margin: auto;
    width: 100%;
    text-align: center;
}

.team h5 {
    font-size: 14px;
    text-align: center;
    padding-top: 10px;
}

.tab_mode h5 {
    display: inline-block;
    font-size: 13px;
    margin-top: 30px;
    font-weight: bold;
}

.h5_format {
    color: #989898;
    margin-left: 30px;
}


.create_tab {
    background: #FFFFFF;
    border-radius: 8px;
    height: 65px;
    width: 100%;
}

.display_design {
    align-items: center;
    display: flex;

}

.display_design h3 {
    font-size: small;
    margin: 10px;

}

.food_class h3 {
    background: #F6F6F6;
    border-radius: 10px;
    padding: 16px;

}

.font_design {
    display: flex;
    align-items: center;
}

.font_design h3 {
    background: #E7DEFA;
    border-radius: 4px;
    font-size: 10px;
    margin-top: 10px;
    padding: 10px;
}

.font_design i {
    margin: 0px 10px;
    color: #989898;
}




.toggleBn {
    width: 10%;
    margin: auto;
}

body.dark {
    background-color: #292c35;
}

/* #9b59b6 */

body.dark h1,
body.dark .support a {
    color: #fff;
}

.checkbox {
    opacity: 0;
    position: absolute;
}

.checkbox-label {
    background-color: #111;
    width: 50px;
    height: 26px;
    margin: 30px auto;
    border-radius: 50px;
    position: relative;
    padding: 5px;
    cursor: pointer;
    display: flex;
    justify-content: space-between;
    align-items: center;
}

.fa-moon {
    color: #f1c40f;
}

.fa-sun {
    color: #f39c12;
}

.checkbox-label .ball {
    background-color: #fff;
    width: 22px;
    height: 22px;
    position: absolute;
    left: 2px;
    top: 2px;
    border-radius: 50%;
    transition: transform 0.2s linear;
}

.checkbox:checked+.checkbox-label .ball {
    transform: translateX(24px);
}

/*  Support me if you like it */
.support {
    position: absolute;
    right: 20px;
    bottom: 20px;
}

.support a {
    color: #292c35;
    font-size: 32px;
    backface-visibility: hidden;
    display: inline-block;
    transition: transform 0.2s ease;
}

.support a:hover {
    transform: scale(1.1);
}
</style>