<template lang="html">
    <div class="chat-log">
        <chat-message v-for="message in messages" :message="message"> </chat-message>
    </div>
</template>


<script>
    export default {
        mounted() {
            console.log('Component ChatLog mounted.')
        },

        props: ['messages']
    }
</script>


<style lang="css">

    .chat-log .chat-message:nth-child(even){
        background-color: #ccc;
    }

</style>
