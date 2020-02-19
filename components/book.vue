<template>
    <article class="book" v-bind:style="{ backgroundColor: color }">
        <section class="bg"></section>
        <section class="content">
        <aside></aside>
        <section>
            <h2>{{ title }}</h2>
            <h3>{{ author }}</h3>
        </section>
        </section>
    </article>
</template>

<script>
export default {
    name: 'book',
    props: {
        book: Object
    },
    computed: {
        title() {
            return this.book.title;
        },
        author() {
            return this.book.author;
        },
        color() {
            return this.book.color;
        }
    }
}
</script>

<style>

</style>