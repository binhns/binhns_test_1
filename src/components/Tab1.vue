<template>
    <div class="grid grid-flow-row grid-cols-1 md:grid-cols-3 ">
        <div class="">
            <div class="text">
                Graphite Artist Quality Fine Art Drawing and Sketching Pencils Replaceable Nib Pencils.
            </div>
            <ul class="list">
                <li>MECHANICAL PENCILS</li>
                <li>ARCHITECT'S CHOICE</li>
                <li>EXECUTIVE PENCILS</li>
                <li>ENGRAVABLE PENCILS</li>
            </ul>
            <button class="btn hidden md:block">
                Shop all
            </button>
        </div>
        <div class="col-span-2">
            <div class="sale">
                <div class="percent">
                    25% <span>off</span>
                </div>
                <div class="desc">
                    Offer Applicable on All Our Pencils
                </div>
            </div>

            <div class="products">
                <div class="productsitem">

                    <img src="../assets/img/tabs/pencil1.png" alt="" />
                    <div class="name">
                        <span>Aero</span> Mechanical Pencil
                    </div>
                    <div class="price">
                        $99.00
                        <del>$125.00</del>
                    </div>
                </div>

                <div class="productsitem">

                    <img src="../assets/img/tabs/pencil2.png" alt="" />
                    <div class="name">
                        <span>Castell</span> Mechanical Pencil
                    </div>
                    <div class="price">
                        $75.00
                        <del>$99.00</del>
                    </div>
                </div>

                <div class="productsitem">

                    <img src="../assets/img/tabs/pencil3.png" alt="" />
                    <div class="name">
                        <span>Architect</span> Choice Pencil
                    </div>
                    <div class="price">
                        $45.00
                        <del>$70.00</del>
                    </div>
                </div>
            </div>

            <button class="btn  md:hidden block mx-auto mt-5">
                Shop all
            </button>
        </div>

    </div>
</template>


<style scoped>
.text {
    font-family: 'Poppins', sans-serif;
    font-style: normal;
    font-weight: 400;
    font-size: 21px;
    line-height: 32px;
    text-align: left;
    color: #000000;
    margin-bottom: 20px;
}

ul.list {
    font-family: 'Poppins', sans-serif;
    font-style: normal;
    font-weight: 600;
    font-size: 18px;
    line-height: 40px;
    list-style: disc;
    margin-left: 20px;
    margin-bottom: 35px;
    color: #000000;
    text-align: left;
}

.btn {
    width: 120px;
    height: 50px;

    background: #F4B840;
    border-radius: 5px;

    font-family: 'Poppins', sans-serif;
    font-style: normal;
    font-weight: 700;
    font-size: 14px;
    line-height: 40px;
    text-transform: uppercase;
    color: #FFFFFF;
    transition: all 0.3s;
}

.btn:hover {
    background: #ffaa00;
}

.sale {
    border: 3px solid #FFFFFF;
    border-radius: 18px;
    display: flex;
    margin-bottom: 20px;
}

.sale .percent {
    font-family: 'Poppins', sans-serif;
    font-style: normal;
    font-weight: 700;
    font-size: 36px;
    line-height: 54px;
    /* identical to box height */


    color: #F4B840;
    background-color: #fff;
    width: 200px;
    height: 80px;

    padding: 13px 28px 13px 40px;

}

.sale .desc {
    font-family: 'Poppins', sans-serif;
    font-style: normal;
    font-weight: 300;
    font-size: 25px;
    line-height: 38px;
    color: #000000;
    background: #F4F4F4;
    padding: 13px 28px 13px 24px;
    display: flex;
    align-items: center;

}

.products {
    display: flex;
    justify-content: space-between;
}

.productsitem {
    width: 224px;
    height: 320px;
    background: #FFFFFF;
    border-radius: 18px;

    padding: 10px 20px 34px;
}

.productsitem img {
    width: 180px;
    height: 210px;
    display: block;
    margin: auto;
    margin-bottom: 14px;
}

.productsitem .name {
    font-style: normal;
    font-weight: 500;
    font-size: 14px;
    line-height: 21px;
    text-align: center;

    color: #000000;

    margin-bottom: 7px;

}

.productsitem .price {
    text-align: center;
    font-style: normal;
    font-weight: 600;
    font-size: 16px;
    line-height: 24px;
    /* identical to box height */

    color: #000000;
}

.productsitem .price del {
    font-style: normal;
    font-weight: 400;
    font-size: 14px;
    line-height: 21px;
    text-align: center;
    text-decoration-line: line-through;
    color: #727272;
}

@media(max-width: 767px) {
    .text {
        font-weight: 400;
        font-size: 16px;
        line-height: 27px;
        /* or 169% */
        color: #000000;
    }

    ul.list {
        font-weight: 600;
        font-size: 13px;
        line-height: 32px;
        /* or 246% */
        color: #000000;
        column-count: 2;
        column-gap: 55px;
        margin: 9px;
        white-space: nowrap;
    }

    .sale .percent {
        background-color: #F4F4F4;
        font-size: 36px;
        line-height: 54px;
        padding: 17px 0 19px 21px;
        display: flex;
        align-items: center;
        justify-content: center;
    }

    .sale .percent span {
        font-style: normal;
        font-weight: 700;
        font-size: 18px;
        line-height: 27px;
        padding-bottom: 5px;
        margin-left: 5px;
    }

    .sale .desc {
        font-weight: 400;
        font-size: 16px;
        line-height: 24px;

        color: #000000;
    }

    .products .productsitem:last-child {
        display: none;
    }

    .productsitem {
        width: 165px;
        height: 260px;
        padding: 5px 10px;
        margin: 0 10px;
    }

    .productsitem img {
        width: 135px;
        height: 160px;
        margin-bottom: 0;
    }

    .productsitem .name {
        font-weight: 500;
        font-size: 13px;
        line-height: 18px;
    }

    .productsitem .name span {
        display: block;
    }

    .productsitem .price {
        font-size: 14px;
        line-height: 21px;
    }

    .productsitem .price del {
        font-size: 13px;
        line-height: 20px;
    }

    .btn {
        width: 100px;
        height: 40px;
        font-size: 14px;
    }
}
</style>

