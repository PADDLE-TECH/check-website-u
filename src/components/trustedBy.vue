<template>

    <div class="container-fluid">
        <div class="row">
            <div class="col-E ">
                <h3 class="trust">TRUSTED BY</h3>
                <ul class="trusted-by-logos">
                    <li class="by-logo1"><img src="../assets/images/c-1.png"></li>
                    <li class="by-logo2" ><img src="../assets/images/c-2.png"></li>
                    <li class="by-logo3" ><img src="../assets/images/c-3.png"></li>
                    <li class="by-logo4" ><img src="../assets/images/c-4.png"></li>
                    <li class="by-logo5" ><img src="../assets/images/c-5.png"></li>
                </ul>
            </div>
        </div>
        <div class="row wrap">
            <!--<div class="col-xs-6 by-logo1"><img src="../assets/images/c-1.png"></div>
            <div class="col-xs-6 by-logo2"><img src="../assets/images/c-2.png"></div>-->
            <!--<div class="col-xs-4"></div>
            <div class="col-xs-4"></div>
            <div class="col-xs-4"></div>-->
        </div>
    </div>

    <div class="container-fluid">
        <div class="row" id="table-row">
            <table>
                <tr>
                    <td><img src="../assets/images/c-1.png"></td>
                    <td><img src="../assets/images/c-2.png"></td>
                    <td><img src="../assets/images/c-3.png"></td>
                </tr>
                <tr>
                    <td><img src="../assets/images/c-4.png"></td>
                    <td><img src="../assets/images/c-5.png"></td>
                </tr>
            </table>
            <!--<div class="col-xs-6 by-logo1"><img src="../assets/images/c-1.png"></div>
            <div class="col-xs-6 by-logo2"><img src="../assets/images/c-2.png"></div>-->
        </div>
    </div>
</template>

<script>

</script>

<style scoped>
@import url('http://fonts.cdnfonts.com/css/euclid-circular-a');

* {
    margin: 0%;
    padding: 0%;
    overflow-x: hidden;
}
.col-E {
    text-align: center;
    background-color: #fff;
}
.trust {
    font-family: 'poppins';
    font-style: normal;
    font-weight: 400;
    font-size: 25px;
    line-height: 25px;
    letter-spacing: 0.4em;
    margin-top: 70px;
    overflow-y: hidden;

    font-family: 'Euclid Circular A';

}

li {
    display: inline-block;
    transform: scale(0.5);
    margin-left: -25px;
    margin-right: -25px;
    /*border: 1px  solid red;*/
}
ul {
    transform: translateX(-30px);
    margin-top: -95px;
    margin-bottom: 80px;
}

/*.trusted-by-logos {
    margin-top: 30px;
    transform: scale(1.5);
}
.by-logo {
    margin-left: 40px;
    margin-right: 40px;
}*/
    table {
        display: none;
    }

@media screen and (min-width: 576px) and (max-width: 768px) {
    #table-row {
        /*text-align: center;*/
        display: flex;
        justify-content: center;
        align-items: center;
    }
    ul {
        transform: translateX(0px);
        margin-top: -0px;
        margin-bottom: 0px;
        white-space: nowrap;

        display: none;
    }
    table {
        margin-top: 50px;
        display: inline-block;
        margin-left: 60px;
        /*margin: 0 auto;*/

    }
    td img {
        width: 170px;
        height: 170px;
    }
    td{
        /*border: 1px solid green;*/
        padding: 20px;
    }
}

@media screen and (max-width: 425px) {
    ul {
        transform: translateX(0px);
        margin-top: -0px;
        margin-bottom: 0px;
        white-space: nowrap;

        display: none;
    }
    li {
        transform: scale(0.2);
        display: inline-block;
        margin-left: -150px;
        margin-right: -10px;
        padding: 0px;

    }
    .wrap {
        white-space: nowrap;
    }
    .col-xs-6 {
        transform: scale(0.2);
        display: inline-block;
    }

    td{
        /*border: 1px solid green;*/
        padding: 20px;
    }
    td img {
        width: 60px;
        height: 60px;
    }
    table {
        margin-top: 50px;
        display: inline-block;
        margin-left: 20px;

    }
    tr {
        display: flex;
        justify-content: center;
        align-items: center;
    }

}


</style>