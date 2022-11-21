<template>
    <div class="wrapper">
        <div class="mycontainer">
            <div class="container-lg py-5">
                <div class="pb-5">
                    <div class="uptitle">Articles and Tips</div>
                    <h2 class="text-center">Latest from the blog</h2>
                </div>
                <div class="row gx-5 ">
                    <div class="col">
                        <div class="mycard  top-50">
                            <img src="/images/120084500_197897808368764_8114555493043279565_n.jpg" alt=""
                                class="img-fluid">
                            <div class="body-mycard p-2">

                                <div class="text-secondary">ARTIST</div>
                                <h3>Brush Stokes Energize</h3>
                                <div class="text-secondary">May 15, 2020</div>
                            </div>
                        </div>
                    </div>
                    <div class="col-6">
                        <div class="mycard center position-relative"><img src="/images/artist-blog-02-500x680.jpg"
                                alt="" class="">
                            <div class=" position-absolute bottom-0 p-3">
                                <div class="text-secondary">ARTIST</div>
                                <h3>Brush Stokes Energize</h3>
                                <div class="text-secondary">May 15, 2020</div>
                            </div>
                        </div>
                    </div>
                    <div class="col">
                        <div class="mycard">
                            <img src="/images/artist-blog-01-480x356.jpg" alt="" class="img-fluid">
                            <div class="body-mycard p-2">
                                <div class="text-secondary">ARTIST</div>
                                <h3>Brush Stokes Energize</h3>
                                <div class="text-secondary">May 15, 2020</div>
                            </div>
                        </div>
                    </div>
                </div>
            </div>
        </div>
    </div>
</template>

<script>
export default {
    name: 'ArticlesTipsComp',
    data() {
        return {

        }
    },
}
</script>

<style lang="scss" scoped>
@use '../assets/style/partials/variables' as *;

.wrapper {
    padding: 1rem 0;
    background-color: $grey-Articles-Tips;
    // height: 100vh;
    background-image: url('/images/maxcoach-shape-03.png');
    background-size: 100%;

    background-position: center;
    background-repeat: no-repeat;

    .mycontainer {
        max-width: 1100px;

    }

    // filter: hue-rotate(90deg);
    .mycard {
        // width: 200px;
        background-color: $white;
        box-shadow: 0px 0px 10px 1px rgba(103, 103, 103, 0.406);



        img {
            // max-width: 100%;
        }
    }



}

.mycard.center {
    overflow: hidden;

    img {
        width: 105%;
        object-fit: cover;
    }
}

.col:first-child {
    align-self: center;
}

.col:last-child {
    position: relative;
    top: 80px;
    // height: 100%;


}
</style>