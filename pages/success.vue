<template>
    <div class="container-fluid">
   <!--      <h5>Logo</h5> -->

        <div class="congrat mt-5">
            <h5>Welcome On Board </h5>
            <h3><br><span style="padding-top: 13px; color: #FFFFFF;"><i class="fa fa-spinner fa-3x fa-spin"></i> </span></h3>
            <img src="../assets/moplexlogo.png" alt="welcome" style="margin-top: 120px;">
        </div>

    </div>
</template>

<script setup>
import { ref, onMounted } from 'vue'

onMounted(() => {
   // console.log('Component mounted!')
    const router = useRouter()
    setTimeout(() => router.push('/home'), 4000);
})
</script>

<style scoped>
.container {
    background: rgba(0, 0, 0, 0.8);
    width: 100%;
    height: 100vh;
}

.container h5 {
    padding: 10px 30px;
    font-size: 40px;
}

.congrat {
    width: 50%;
    margin: auto;
    text-align: center;
}

.congrat h5 {
    font-size: 50px;
    color: #ffffff;
    margin: 0px;
    font-weight: bolder;
}

@media only screen and (max-width: 600px) {

    .congrat {
        width: 100%;
        margin: auto;
        text-align: center;

    }

    .container h5 {
        padding: 0px 0px;
        font-size: 20px;
        text-align: center;
    }

    .congrat img {
        width: 100%;

    }

    .container h5 {
        padding: 10px 30px;
        font-size: 20px;
    }

}
</style>