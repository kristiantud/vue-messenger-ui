<template>
    <div>
        <div style="padding: 30px 15px; background-color: #606060" class="msg-preview" v-if="selected === id">
            <p><b>{{ sender }}</b></p>
            <p>{{ msgs[0].content }}</p>
        </div>
        <div style="padding: 30px 15px" class="msg-preview" v-else>
            <p><b>{{ sender }}</b></p>
            <p>{{ msgs[0].content }}</p>
        </div>
        
    </div>
    
    
    <hr>
</template>

<script>

    export default {
        name: 'MessagePreviews',
        props: {
            sender: String,
            msgs: Array,
            id: Number,
            selected: Number,
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