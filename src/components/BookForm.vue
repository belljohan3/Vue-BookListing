<template>
    <div>
        <form v-on:submit.prevent="bookSubmit(bookTitle, bookAuthor)" class="" action="#" method="post">
            <input v-model="bookTitle" type="text" name="title" placeholder="Book Title">
            <input v-model="bookAuthor" type="text" name="author" placeholder="Book Author">
            <button type="submit" name="button">Add Book</button>
        </form>
    </div>
</template>
<script>
export default {
    name: 'BookForm',
    props: ['books'],
    data() {
        return {
            bookTitle: '',
            bookAuthor: ''
        }
    },
    methods: {
        bookSubmit (booktitle, bookTitle){
            this.$emit('addBook', bookTitle, bookAuthor);
        },
        bookTitle () {

        },
        bookAuthor () {

        }
    },
}
</script>
<style>
    
</style>