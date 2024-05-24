<script>
export default {
    data() {
        return {
            dcComics: [
                'Characters',
                'Comics',
                'Movies',
                'TV',
                'Games',
                'Videos',
                'News'
            ],
            dc: [
                'Terms Of House',
                'Privacy Policy (New)',
                'Ad Choices',
                'Advertising',
                'Jobs',
                'Subscriptions',
                'Talent Workshop',
                'CPSC Certificates',
                'Ratings',
                'Shop Help',
                'Contact Us'
            ],
            sites: [
                'DC',
                'MAD Magazine',
                'DC Kids',
                'DC Universe',
                'DC Power Visa'
            ],
            shop: [
                'Shop DC',
                'Shop DC ollectibles'
            ],
        }
    }
}

</script>

<template>
    <div class="contenitore">

        <div class="d-flex justify-content-between" style="height: 100%;">
            <div class="left-side d-flex justify-content-between" style="width: 25%;">
                <div class="subtitle">
                    <h6 class="my_fs-t text-nowrap">DC COMICS</h6>
                    <ul class="m-0 p-0">
                        <li class="my_fs-l" v-for="elemento in dcComics">{{ elemento }}</li>
                    </ul>
                    <h6 class="my_fs-t mt-3 text-nowrap">SHOP</h6>
                    <ul class="m-0 p-0">
                        <li class="my_fs-l" v-for="elemento in shop">{{ elemento }}</li>
                    </ul>
                </div>
                <div class="subtitle">
                    <h6 class="my_fs-t text-nowrap">DC</h6>
                    <ul class="m-0 p-0">
                        <li class="my_fs-l" v-for="elemento in dc">{{ elemento }}</li>
                    </ul>
                </div>
                <div class="subtitle">
                    <h6 class="my_fs-t text-nowrap">SITES</h6>
                    <ul class="m-0 p-0">
                        <li class="my_fs-l" v-for="elemento in sites">{{ elemento }}</li>
                    </ul>
                </div>
            </div>
            <div class="right-side " style="width: 60%;">

            </div>
        </div>

    </div>
</template>

<style scoped>
.contenitore {
    color: white;
}

.subtitle {
    width: calc(100% / 3 - 3rem);
    margin: 2rem 0.5rem;
}

li {
    list-style-type: none;
}

.my_fs-t {
    font-size: 0.8rem;
    font-weight: bold;
}

.my_fs-l {
    font-size: 0.5rem;
    font-weight: bold;
    color: grey;
}

.right-side {
    background-image: url(../assets/img/dc-logo-bg.png);
    background-repeat: no-repeat;
    background-position: right;
}
</style>