<template>
    <div class="container-fluid">
        <div class="row">
            <div class="col-sm-2 m-0 p-0">

                <header>

                    <ul class="pt-3">
                        <li><img src="../assets/d.png" alt=""> <span
                                style=" margin-left: 10px; font-weight: bold;">Cube</span> <span
                                style="margin-left: 50px;"><i class="fa fa-bell m"></i></span> <img src="../assets/e.png"
                                alt=""> </li>
                    </ul>


                    <ul class="mt-4">
                        <div class="nav_style">
                            <li><i class="fa fa-home" style="margin-right: 10px;"></i> Home</li>
                            <li><i class="fa fa-envelope" style="margin-right: 10px;"></i> Inbox</li>
                            <li><i class="fa fa-circle" style="margin-right: 10px;"></i> Search</li>
                            <li><i class="fa fa-plus-circle" style="margin-right: 10px;"></i>New Feedback</li>
                        </div>
                    </ul>

                    <ul class="mt-4">
                        <li style="color: #989898;"><i class="fa fa-caret-down" style="margin-right: 10px;"></i> Main Boards
                        </li>
                        <div class="nav_style">
                            <li><i class="fa fa-home" style="margin-right: 10px;"></i> Road Maps</li>
                            <li><i class="fa fa-envelope" style="margin-right: 10px;"></i>Release Notes</li>
                            <li><i class="fa fa-plus-circle" style="margin-right: 10px;"></i> Add View</li>
                        </div>
                    </ul>


                    <ul class="mt-4">
                        <li style="color: #989898;"><i class="fa fa-caret-down" style="margin-right: 10px;"></i> Design
                            boards </li>
                        <div class="nav_style">
                            <li><i class="fa fa-home" style="margin-right: 10px;"></i>Design System</li>
                            <li><i class="fa fa-envelope" style="margin-right: 10px;"></i>Cube Design Team</li>
                            <li><i class="fa fa-plus-circle" style="margin-right: 10px;"></i>Cube 2.0</li>
                            <li><i class="fa fa-plus-circle" style="margin-right: 10px;"></i>Add View</li>
                        </div>
                    </ul>


                    <ul class="mt-4">
                        <li style="color: #989898;"><i class="fa fa-caret-down" style="margin-right: 10px;"></i> Main Board
                        </li>
                        <div class="nav_style">
                            <li><i class="fa fa-home" style="margin-right: 10px;"></i> Front-end</li>
                            <li><i class="fa fa-envelope" style="margin-right: 10px;"></i>Back-end</li>
                            <li><i class="fa fa-plus-circle" style="margin-right: 10px;"></i>Bugs</li>
                            <li><i class="fa fa-plus-circle" style="margin-right: 10px;"></i>Add View</li>
                        </div>
                    </ul>


                    <ul class="mt-4">
                        <li style="color: #989898;"><i class="fa fa-caret-down" style="margin-right: 10px;"></i> Other Views
                        </li>
                        <div class="nav_style">
                            <li><i class="fa fa-home" style="margin-right: 10px;"></i> Target</li>
                            <li><i class="fa fa-plus-circle" style="margin-right: 10px;"></i>Add View</li>
                        </div>
                    </ul>



                    <!--   <div class="user-id">
                        <div class="user-name ">
                            Main boards
                        </div>
                        <div class="dropdown-arrow"></div>
                        <div class="dropdown-menu">
                            <ul>
                                <li><i class="fa fa-home" style="margin-right: 10px;"></i> Road Map</li>
                                <li><i class="fa fa-envelope" style="margin-right: 10px;"></i> Release Note</li>
                                <li><i class="fa fa-circle" style="margin-right: 10px;"></i> Add View</li>
                            </ul>
                        </div>

                    </div>

                    <div class="user-id">
                        <div class="user-name ">
                            Design boards
                        </div>
                        <div class="dropdown-arrow"></div>
                        <div class="dropdown-menu">
                            <ul>
                                <li><i class="fa fa-home" style="margin-right: 10px;"></i>Design System</li>
                                <li><i class="fa fa-envelope" style="margin-right: 10px;"></i> Cube Design Sysytem</li>
                                <li><i class="fa fa-circle" style="margin-right: 10px;"></i> Cube 2.0</li>
                            </ul>
                        </div>

                    </div>

                    <div class="user-id">
                        <div class="user-name ">
                            Developer
                        </div>
                        <div class="dropdown-arrow"></div>
                        <div class="dropdown-menu">
                            <ul>
                                <li><i class="fa fa-home" style="margin-right: 10px;"></i> Road Map</li>
                                <li><i class="fa fa-envelope" style="margin-right: 10px;"></i> Release Note</li>
                                <li><i class="fa fa-circle" style="margin-right: 10px;"></i> Add View</li>
                            </ul>
                        </div>

                    </div>


                    <div class="user-id">
                        <div class="user-name ">
                            Other Views
                        </div>
                        <div class="dropdown-arrow"></div>
                        <div class="dropdown-menu">
                            <ul>
                                <li><i class="fa fa-home" style="margin-right: 10px;"></i> Target</li>
                                <li><i class="fa fa-circle" style="margin-right: 10px;"></i> Add View</li>
                            </ul>
                        </div>

                    </div -->

                    <ul class="mt-4">
                        <div class="nav_style">
                            <li><i class="fa fa-home" style="margin-right: 10px;"></i> Learning Center</li>
                            <li><i class="fa fa-envelope" style="margin-right: 10px;"></i>Contact Support</li>
                            <li><i class="fa fa-plus-circle" style="margin-right: 10px;"></i> Invite New Member</li>
                        </div>
                    </ul>







                </header>



                <nav v-if="mob_Tab != ''">

                    <ul style="margin-top: 8rem">
                        <router-link to="/">
                            <li>
                                <i class="fas fa-house-medical fa-1x"></i><span class="ml-3">Dashboard</span>
                            </li>
                        </router-link>
                    </ul>
                    <ul>
                        <router-link to="/patientrec">
                            <li>
                                <i class="fa-solid fa-user-doctor"></i> <span class="ml-3">Manage Patients</span>
                            </li>
                        </router-link>
                    </ul>

                    <ul v-if="user_type == 'Physician'">
                        <router-link to="/physician">
                            <li>
                                <i class="fa-solid fa-user-doctor"></i><span class="ml-3">Manage Physicians</span>
                            </li>
                        </router-link>
                    </ul>
                    <ul v-if="user_type == 'Physician'">
                        <router-link to="/nurse">
                            <li>
                                <i class="fa-solid fa-user-nurse"></i><span class="ml-3">Manage Nurses</span>
                            </li>
                        </router-link>
                    </ul>
                    <ul>
                        <router-link to="/physicianorder">
                            <li>
                                <i class="fa-solid fa-stethoscope"></i><span class="ml-3">Physician Order</span>

                            </li>
                        </router-link>
                    </ul>
                    <ul>
                        <router-link to="/classification">
                            <li>
                                <i class="fa fa-pills"></i><span class="ml-3">Classification Order</span>
                            </li>
                        </router-link>
                    </ul>
                    <ul> <router-link to="/vent">
                            <li>
                                <i class="fa fa-pills"></i><span class="ml-3">Ventilator</span>
                            </li>
                        </router-link></ul>

                    <ul class="mt-5">
                        <router-link to="#">
                            <li @click="logOut()"><i class="fa fa-sign-out"></i><span class="ml-3">Log Out</span></li>
                        </router-link>

                    </ul>





                </nav>









            </div>

            <div class="col-sm-10 m-0 p-0 bg-dark">
                
                <div>
                    <slot />
                </div>
            </div>
        </div>
    </div>







    <!--  Output the page content -->


    <!--  Output the page content -->
</template>

<style scoped>
nav{
    display: none;
}
header {
    background: #FFFFFF;
    box-shadow: 0px 0px 8px rgba(0, 0, 0, 0.1);
    padding-bottom: 20px;
    height: 100vh;
    overflow: scroll;
    overflow: -moz-scrollbars-none;
    -ms-overflow-style: none;
    scrollbar-width: none;

    box-sizing: border-box;
    -ms-overflow-style: none !important;
    /* for Internet Explorer, Edge */
}

header::-webkit-scrollbar {
    display: none;
}

ul {
    list-style: none;
    cursor: pointer;
}


.nav_style li {

    width: 90%;
    padding: 8px 5px;
    font-size: 12px;
}

.nav_style li:hover {
    background: #1CA19E;
    width: 90%;
    padding: 8px 5px;
    border-radius: 12px;
}

.user-id {
    height: 100px;
    width: 100%;
    background: #fff;
    position: relative;
    cursor: pointer;
}


.user-name {
    line-height: 2.5em;
    padding: 0px;
    text-align: center;
    margin-right: 3px;
}

.dropdown-arrow {
    height: 0;
    width: 0;
    border-left: 10px solid transparent;
    border-right: 10px solid transparent;
    border-top: 10px solid #333;
    position: relative;
    left: 35px;
    bottom: 22px;
}

.user-id:hover .dropdown-arrow {
    border-left: 10px solid transparent;
    border-right: 10px solid transparent;
    border-bottom: 10px solid #333;
    border-top: 10px solid transparent;
    bottom: 32px;
}

.dropdown-menu {
    list-style-type: none;
    display: none;
    top: 30px;
    border: none;



}

.user-id:hover .dropdown-menu {
    display: block;
    position: absolute;
}

.dropdown-menu ul li {
    list-style-type: none;
    display: block;
    padding: 5px;
    border: none;
}

.dropdown-menu ul li:last-child {
    border-bottom: none;
}

.dropdown-menu ul li:hover {
    border: none;
    border-bottom: none;

}




@media only screen and (max-width: 600px) {

    header {
        display: none;
    }

}</style>