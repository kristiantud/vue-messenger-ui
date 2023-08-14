<template>
    <div style="padding: 30px 15px" class="msg-preview">
        <p><b>{{ sender }}</b></p>
        <p>{{ msgs[0].content }}</p>
    </div>
    <hr>
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

<style scoped>
*{
    font-family:Arial, Helvetica, sans-serif;
    font-size: 15px;
}

hr{
    border: solid thin white;
    padding: 0;
    margin: 0;
}    

.msg-preview p{
    color: white;
}


.msg-preview:hover {
  cursor: pointer;
  background-color: #353535;
}

</style>