<template>
    <div class="container-fluid">
        <div class="row">
            <div class="col-sm-2 m-0 p-0">
                <header>

                    <ul class="pt-3">
                        <NuxtLink to="/home">
                            <li><img src="../assets/moplexlogo.png" alt="" style="width: 75%;"> <!-- <span
                                    style="margin-left: 30px;"><i class="fa fa-bell m"></i></span> <img
                                    src="../assets/e.png" alt="">  --></li>
                        </NuxtLink>

                    </ul>


                    <ul class="mt-4">
                        <div class="nav_style">
                            <NuxtLink to="/home">
                                <li><i class="fa fa-home" style="margin-right: 10px;"></i> Home</li>
                            </NuxtLink>
                            <li><i class="fa fa-envelope" style="margin-right: 10px;"></i> Inbox</li>
                            <li><i class="fa fa-circle" style="margin-right: 10px;"></i> Search</li>
                            <li><i class="fa fa-plus-circle" style="margin-right: 10px;"></i>New Feedback</li>
                        </div>
                    </ul>

                    <ul class="mt-4">
                        <li style="color: #989898;"><i class="fa fa-caret-down" style="margin-right: 10px;"></i> Movies
                        </li>
                        <div class="nav_style">
                            <li data-bs-toggle="modal" data-bs-target="#exampleModal">
                                <i class="fa fa-film" style="margin-right: 10px;"></i>
                                Add New
                            </li>
                            <NuxtLink to="/movies">
                                <li><i class="fa fa-envelope" style="margin-right: 10px;"></i>All Movies</li>
                            </NuxtLink>

                            <li><i class="fa fa-plus-circle" style="margin-right: 10px;"></i> Add View</li>
                        </div>
                    </ul>


                    <ul class="mt-4">
                        <li style="color: #989898;"><i class="fa fa-caret-down" style="margin-right: 10px;"></i>Credentials </li>
                        <div class="nav_style">
                            <Nuxt-link to="/user">
                                <li><i class="fa fa-user" style="margin-right: 10px;"></i>Add User</li>
                            </Nuxt-link>

                            <Nuxt-link to="/userstab">
                                <li><i class="fa fa-envelope" style="margin-right: 10px;"></i>Manage Users</li>
                            </Nuxt-link>
                        
                        </div>
                    </ul>


                    <ul class="mt-4">
                        <li style="color: #989898;"><i class="fa fa-caret-down" style="margin-right: 10px;"></i> Main Board
                        </li>
                        <div class="nav_style">
                            <li><i class="fa fa-home" style="margin-right: 10px;"></i>Log Out</li>
                        </div>
                    </ul>

                </header>

                <!-- Modal -->
                <div class="modal fade" id="exampleModal" tabindex="-1" aria-labelledby="exampleModalLabel"
                    aria-hidden="true">
                    <div class="modal-dialog">
                        <div class="modal-content">
                            <div class="modal-header">
                                <h5 class="modal-title" id="exampleModalLabel">Choose Movie Type</h5>
                                <button type="button" class="btn-close" data-bs-dismiss="modal" aria-label="Close"></button>
                            </div>
                            <div class="modal-body">
                                <NuxtLink to="/movie"><button class="next_btn btn" data-bs-dismiss="modal"
                                        aria-label="Close">
                                        Produced Movie

                                    </button></NuxtLink>
                                <!--   <NuxtLink to="/movie" data-bs-dismiss="modal" aria-label="Close"></NuxtLink>
                                <NuxtLink to="/movieprod" data-bs-dismiss="modal" aria-label="Close">Purchased Movie
                                </NuxtLink> -->
                                <NuxtLink to="/movieprod"><button class="next_btn btn" data-bs-dismiss="modal"
                                        aria-label="Close">
                                        Purchased Movie

                                    </button></NuxtLink>
                            </div>
                        </div>
                    </div>
                </div>

            </div>

            <div class="col-sm-10 m-0 p-0 bg-dark">
                <slot />
            </div>

            <!-- Fix AND Fox Modal -->
        </div>
    </div>







    <!--  Output the page content -->


    <!--  Output the page content -->
</template>

<style scoped>
a {
    text-decoration: none;
    color: white;
}

nav {
    display: none;
}

header {
    background: rgba(30, 30, 30, 0.8);
    box-shadow: 0px 0px 8px rgba(0, 0, 0, 0.1);
    padding-bottom: 20px;
    height: 100vh;
    overflow: scroll;
    overflow: -moz-scrollbars-none;
    -ms-overflow-style: none;
    scrollbar-width: none;
    color: white;
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
    padding: 9px 5px;
    font-size: 15.5px;
}

.nav_style li:hover {
    background: red;
    width: 90%;
    padding: 9px 5px;
    border-radius: 12px;
}
/* .nav_style a.router-link-active{
    background: red;
    width: 90%;
    padding: 9px 5px;
    border-radius: 12px;
} */
/* .nav_style a:active {
    background: red;
    width: 90%;
    padding: 9px 5px;
    border-radius: 12px;
} */

/* .nav_style a.router-link-exact-active {
    background: red;
    width: 90%;
    padding: 9px 5px;
    border-radius: 12px;
} */


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

.btn-close:focus {
    box-shadow: none !important;
}

/* .modal-body a {
    color: black;
    display: block;
    text-align: center;
    margin: 20px auto;
    padding: 10px;
    width: 200px;
    cursor: pointer;
} */

.next_btn {
    color: black;
    display: block;
    text-align: center;
    margin: 20px auto;
    padding: 10px;
    width: 200px;
    cursor: pointer;
    border: none;
}

.next_btn:hover {
    background: red;
    border-radius: 5px;
    padding: 10px;
    margin: 20px auto;
    width: 200px;
    border: none;
    color: white;

}

@media only screen and (max-width: 600px) {

    header {
        display: none;
    }

}
</style>