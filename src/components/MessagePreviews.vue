<template>
    <div>
        {{ sender }}
        {{ msgs[0].content }}
        
    </div>
</template>

<script>

    export default {
        name: 'MessagePreviews',
        props: {
            sender: String,
            msgs: Array,
        }
    }

</script>
