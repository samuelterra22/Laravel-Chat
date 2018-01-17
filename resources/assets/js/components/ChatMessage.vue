<template lang="html">
    <div class="chat-message">
        <p>{{ message.message }}</p>
        <small>{{message.user}}</small>
    </div>
</template>


<script>
    export default {
        mounted() {
            console.log('Component ChatMessage mounted.')
        },

        props: ['message']
    }
</script>


<style lang="css">

    .chat-message{
        padding: 1rem;
    }

    .chat-message > p{
        margin-bottom: .5rem;
    }

</style>
