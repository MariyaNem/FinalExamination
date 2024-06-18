<template>
    <div class="bgr bgsize">
        <div class="subscribe">
            <div class="row">
                <div class="col-md-12">
                    <h1 class="subscribe__title ">Записаться на консультацию</h1>
                    <form class="row g-3 needs-validation" novalidate>
                        <div class="col-md-4">
                            <label for="validationCustom01" class="form-label subscribe__text">Ваше Имя</label>
                            <input type="text" class="form-control subscribe__input" id="validationCustom01" required>
                        </div>
                        <div class="col-md-4">
                            <label for="validationDefault03" class="form-label subscribe__text">Номер телефона</label>
                            <input type="text" class="form-control subscribe__input" id="validationDefault03" required>
                        </div>

                        <div class="col-md-4">
                            <label for="validationCustom04" class="form-label subscribe__text">Клиника для
                                записи</label>
                            <select class="form-select subscribe__input" id="validationCustom04" required>
                                <option selected disabled value="">Выберите..</option>
                                <option>Пр. Проспектовый, 4</option>
                                <option>Ул. Уличная, 5</option>
                            </select>
                        </div>

                        <div class="d-grid gap-2">
                            <button class="btn  btn-outline-light subscribe__button" type="button">Записаться!</button>
                        </div>

                    </form>
                </div>
            </div>
        </div>
    </div>
</template>


<style>
.bgr {
    background-image: url(../assets/images/bg/subscribe.png);
    background-size: cover;
}
</style>