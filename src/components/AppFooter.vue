<script>
export default {
    data() {
        return {
            socialIcons: [
                '../../img/footer-facebook.png',
                '../../img/footer-twitter.png',
                '../../img/footer-youtube.png',
                '../../img/footer-pinterest.png',
                '../../img/footer-periscope.png',
            ]
        }
    }
}


</script>

<template>
    <div class="contenitore">

        <div class="d-flex justify-content-between" style="height: 100%;">
            <div class="left-side align-content-center text-center" style="width: 10%;">
                <div>
                    <h6 class="my_fs m-0 border border-primary text-nowrap p-2">SIGN-UP NOW</h6>
                </div>
            </div>
            <div class="right-side align-content-center" style="width: 30%;">
                <span class="me-3 text-primary">FOLLOW US</span class="me-2">
                <img v-for="immagine in socialIcons" :src="immagine" alt="">
            </div>
        </div>

    </div>
</template>

<style scoped>
.contenitore {
    color: white;
}

.my_fs {
    font-size: 0.8rem;

}

img {
    margin: 0 0.4rem;
}
</style>