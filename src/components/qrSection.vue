<template>

    <div class="container-fluid">
        <div class="row qrSection">
            <aos-vue animation="fade-right" class="col-md-7 col-sm-4"><img src="../assets/images/woman-ii.webp" class="woman"></aos-vue>
            <div class="col-md-5 col-sm-8">
                <h1 class="QR"><b>A QR technology enhanced future</b></h1>
                <p class="you-are">You are  here because the future matters. We  thought  of what you need and expressed it in this beautiful piece of technology.</p>
                <button class="btn2">Download Now</button>
            </div>
        </div>
    </div>


</template>

<script>

</script>

<style scoped>
@import url('http://fonts.cdnfonts.com/css/euclid-circular-a');

.container-fluid {
    overflow-x: hidden;
    font-family: 'Euclid Circular A';
}
.row {
    background-color: rgb(248, 242, 248);
    width: 100vw;
}
.woman {
    width: 805px;
    height: 685px;
}
.QR {
    font-family: 'poppins';
    font-style: normal;
    font-weight: 600;
    font-size: 75px;
    line-height: 80px;
    letter-spacing: -0.05em;
    background: linear-gradient(90deg, rgba(254,64,149,1) 0%, rgba(242,180,159,1) 64%, rgba(163,90,195,1) 90%);
    -webkit-background-clip: text;
    -webkit-text-fill-color: transparent;
    background-clip: text;
    /*max-width: 480px;*/
    text-align: left;
    letter-spacing: 1px;

    margin-top: 80px;
    padding-left: 30px;
    font-family: 'Euclid Circular A';
}

.you-are {
    font-family: 'poppins';
    font-style: normal;
    font-weight: 300;
    font-size: 20px;
    line-height: 25px;
    margin-left: 30px;

    text-align: left;
    padding-left: 0px;
    margin-top: 20px;
    width: 452px;
    font-family: 'Euclid Circular A';
}
.col-md-5 {
    margin-right: 0px;
    text-align: left;
}
.btn2 {
    font-family: 'poppins';
    font-style: normal;
    font-weight: 500;
    font-size: 25px;
    line-height: 38px;
    padding: 15px 65px 16px 65px;
    color: #fff;
    background-color: black;
    margin-left: 30px;
    margin-top: 34px;
    font-family: 'Euclid Circular A';

    border-radius: 10px;
    transition: all 0.4s ease;
}
.btn2:hover {
    transform: scale(1.03);
    opacity: 0.9;
    transition: all 0.4s ease;
}

@media screen and (max-width: 425px){
    .woman {
        width: 355px;
        height: 255px;
        margin-top: 50px;

        margin-right: 20px;
    }
    .QR {
        /*font-size: 56.5px;*/
        font-size: 45px;
        line-height: 43px;
        padding-left: 20px;
        margin-right: 0px;
    }
    .you-are {
        width: 322px;
        margin-left: 20px;
    }
    .btn2 {
        margin-left: 20px;
    }
    .qrSection {
        margin-bottom: 50px;
    }

}

@media screen and (min-width: 576px) and (max-width: 768px) {
    .woman {
        width: 455px;
        height: 455px;
        margin-top: 50px;

        margin-right: 40px;
        transform: translateX(-10px);
    }
    .QR {
        /*font-size: 56.5px;*/
        font-size: 45px;
        line-height: 43px;
        padding-left: 20px;
        margin-right: 0px;
    }
    .you-are {
        width: 322px;
        margin-left: 20px;
    }
    .btn2 {
        margin-left: 20px;
        padding: 15px 25px 16px 25px;
    }
    .qrSection {
        margin-bottom: 50px;
    }
    .col-md-5 {
        margin-left: -20px;
    }

}

</style>