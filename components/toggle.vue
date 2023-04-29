<template>
    <div class="container-fluid">
        <div class="row">
            <div class=" col-sm-11 mx-auto pt-3">
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
        </div>
    </div>
</template>
<script setup >
import { ref, defineEmits } from 'vue';

const isActive = ref(false);

const toggleDarkMode = () => {
    //  home.value = !home.value;

    if (isActive.value) {
        isActive.value = false;
    } else {
        isActive.value = true;
    }
}

defineEmits
/*  return { isActive, toggleDarkMode }; */


</script>


<style scoped>
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