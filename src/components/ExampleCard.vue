<script>

    export default {
        name: "Example Card",
        props: ['name', 'image', 'paragraph'],

        data() {
            return {
                onHover: false,
            };
        },

        methods: {

            hoverEffect() {
                this.onHover = true;
                console.log("funziono");
            },

        }

    };

</script>

<template>

    <div @mouseenter="hoverEffect()" :class="{ hover: this.onHover }" class="card text-bg-dark border-0">
        <img
            :src="image"
            class="card-img"
            :alt="name"
        />
        <div class="card-img-overlay d-flex flex-column justify-content-end p-5" v-show="onHover === true">
            <h5 class="card-title fs-4 fw-semibold">{{ name }}</h5>
            <div class="paragraph">
                <span class="card-text me-3" v-for="element in this.paragraph">{{ element }}</span>
            </div>
        </div>
    </div>

</template>

<style scoped>

.hover {
    color: black;
}

</style>