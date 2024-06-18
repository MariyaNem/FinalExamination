<template>
    <div class="container feature">
        <div>
            <h1 class="feature__blockTitle">Наши врачи</h1>
        </div>
        <div class="row feature__forSecondRow">
            <div class="col-md-3" v-for="item in data" :key="item.id">
                <div class="feature__col">
                    <img class="feature__icon feature__image pic"
                        :src="require(`../assets/images/photos/${item.icons}.png`)" :alt="item.title" />

                    <h4 class="feature__title">{{ item.title }}</h4>
                    <p class="feature__p">{{ item.text }}</p>
                </div>
            </div>
        </div>
    </div>
</template>

<script>
export default {
    props: {
        data: {
            type: Array,
            default: () => []
        },
    },
}
</script>

<style>
.pic {
    height: auto;
    width: 100%;
    max-width: 720px;
}
</style>