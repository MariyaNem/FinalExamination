<template>
    <div id="carouselExampleCaptions" class="carousel slide">
        <div class="carousel-indicators">
            <button type="button" data-bs-target="#carouselExampleCaptions" data-bs-slide-to="0" class="active"
                aria-current="true" aria-label="Slide 1"></button>
            <button type="button" data-bs-target="#carouselExampleCaptions" data-bs-slide-to="1"
                aria-label="Slide 2"></button>
            <button type="button" data-bs-target="#carouselExampleCaptions" data-bs-slide-to="2"
                aria-label="Slide 3"></button>
        </div>
        <div class="carousel-inner">
            <div class="carousel-item active ">
                <img src="../assets/images/slider/slide1.png" class="d-block w-100" alt="">
                <div class="carousel-caption d-none d-md-block width">
                    <h5 class="caruselText">Скажи жизни без кариеса - ДА</h5>
                    <button type="button" class="btn btn-outline-dark button batton">Подробнее</button>

                </div>
            </div>
            <div class="carousel-item">
                <img src="../assets/images/slider/slide2.png" class="d-block w-100" alt="">
                <div class="carousel-caption d-none d-md-block width">
                    <h5 class="caruselText">Положи начало красивой улыбке</h5>
                    <button type="button" class="btn btn-outline-dark button batton">Подробнее</button>
                </div>
            </div>
            <div class="carousel-item">
                <img src="../assets/images/slider/slide3.png" class="d-block w-100" alt="">
                <div class="carousel-caption d-none d-md-block width">
                    <h5 class="caruselText">Инновационные технологии</h5>
                    <button type="button" class="btn btn-outline-dark button batton">Подробнее</button>
                </div>
            </div>
        </div>
        <button class="carousel-control-prev" type="button" data-bs-target="#carouselExampleCaptions"
            data-bs-slide="prev">
            <span class="carousel-control-prev-icon" aria-hidden="true"></span>
            <span class="visually-hidden">Previous</span>
        </button>
        <button class="carousel-control-next" type="button" data-bs-target="#carouselExampleCaptions"
            data-bs-slide="next">
            <span class="carousel-control-next-icon" aria-hidden="true"></span>
            <span class="visually-hidden">Next</span>
        </button>
    </div>
</template>

<style>
.caruselText {
    color: #5565aa;
    font-weight: bold;
    font-size: 30px;
}

.button {
    margin-top: 5px;
}

.width {
    width: 70%;
    height: 23%;
    border-radius: 15px;
    background-color: rgba(255, 250, 250, 0.658);
}
</style>