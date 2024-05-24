<script>

export default {
    data() {
        return {
            otherPages: [
                {
                    text: 'DIGITAL COMICS',
                    immagine: 'buy-comics-digital-comics.png'
                },
                {
                    text: 'DC MERCHANDISE',
                    immagine: 'buy-comics-merchandise.png'
                },
                {
                    text: 'SUBSCRIPTION',
                    immagine: 'buy-comics-subscriptions.png'
                },
                {
                    text: 'COMIC SHOP LOCATOR',
                    immagine: 'buy-comics-shop-locator.png'
                },
                {
                    text: 'DC POWER VISA',
                    immagine: 'buy-dc-power-visa.svg'
                }
            ]
        }
    },
    methods : {
        getImg(path) {
            let risultato = new URL(`../assets/img/` + path, import.meta.url);
            return risultato.href;
        }
    }
}


</script>

<template>
    <div class="contenitore">
        <div class="d-flex" style="height: 100%;">
            <template v-for="page in otherPages">
                <div class="single-card d-flex justify-content-center py-4">
                    <div class="align-content-center">
                        <img :src="getImg(page.immagine)" alt="">
                    </div>
                    <div class="align-content-center px-2 my_fs">
                        {{ page.text }}
                    </div>
                </div>
            </template>


        </div>

    </div>

</template>

<style scoped>
.contenitore {
    color: white;
}

.single-card {
    width: calc(100% / 5);
    text-align: center;
    height: 100%;
}

img {
    height: 100%;
}

.my_fs {
    font-size: 0.7rem;
}
</style>