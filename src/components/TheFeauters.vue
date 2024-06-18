<template>
    <div class="container feature">
        <div class="row feature__forFirstRow">
            <div>
                <h1 class="feature__blockTitle">Наши услуги</h1>
            </div>
            <div class="col-md-3" v-for="item in data" :key="item.id">
                <div class="feature__col">
                    <img class="feature__icon" :src="require(`../assets/images/icons/${item.icons}.png`)"
                        :alt="item.title" />

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