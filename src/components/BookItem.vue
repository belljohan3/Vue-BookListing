<template lang="">
    <div>
        <ul>
            <li>{{book.title}}:{{book.author}}</li>
        </ul>
    </div>
</template>
<script>
export default {
    data() {
        return {
            name: 'BookItem',
            props: ['book']
        }
    },
}
</script>
<style lang="">
    
</style>