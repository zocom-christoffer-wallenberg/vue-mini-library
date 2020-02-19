<template>
  <main class="books">
    <book v-for="(book, index) in books" :key="index" v-bind:book="book" />
  </main>
</template>

<script>
import book from '../components/book'

export default {
    name: 'books',
    components: {
        book
    },
    props: {
        books: Array
    }
}
</script>

<style>
    .books {
        display: grid;
        gap: 1rem;
        grid-template-columns: repeat(4, 1fr);
    }
</style>