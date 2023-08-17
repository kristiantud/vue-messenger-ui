

<!-- will have an array of messages that this loops through -->
<!-- will populate the MsgPrev section of the messageswidget -->

<script>
import MessagePreviews from './MessagePreviews.vue';
import { ref } from 'vue';


    const currentSelected = ref(-1);

    

    export default {
    name: 'MsgPreviewWidget',
    data: function () {
        return {
            currentSelected,
            messages: [
                {
                    id: 1,
                    messages: [
                        { id: "69",
                            sender: "Captain Jack Sparrow",
                            content: "Where's the rum?!" },
                        { id: "70",
                            sender: "somerandomuseridbythesender",
                            content: "How you been???" },
                    ]
                },
                {
                    id: 2,
                    messages: [
                        { id: "69",
                            sender: "Harry Potter",
                            content: "Where's the sorcerer's stone?!" },
                        { id: "70",
                            sender: "somerandomuseridbythesender",
                            content: "How you been???" },
                    ]
                },
                {
                    id: 3,
                    messages: [
                        { id: "69",
                            sender: "J. Robert Oppenheimer",
                            content: "Where's the nuke?!" },
                        { id: "70",
                            sender: "somerandomuseridbythesender",
                            content: "How you been???" },
                    ]
                },
                {
                    id: 4,
                    messages: [
                        { id: "69",
                            sender: "Frodo Baggins",
                            content: "Where's the ring?!" },
                        { id: "70",
                            sender: "somerandomuseridbythesender",
                            content: "How you been???" },
                    ]
                },
                {
                    id: 5,
                    messages: [
                        { id: "69",
                            sender: "Mr. Robot",
                            content: "Where's Angela?!" },
                        { id: "70",
                            sender: "somerandomuseridbythesender",
                            content: "How you been???" },
                    ]
                },
                {
                    id: 6,
                    messages: [
                        { id: "69",
                            sender: "Dr. Strange",
                            content: "Where's the Time Stone?!" },
                        { id: "70",
                            sender: "somerandomuseridbythesender",
                            content: "How you been???" },
                    ]
                },
                {
                    id: 7,
                    messages: [
                        { id: "69",
                            sender: "Itachi",
                            content: "Where's Sasuke?!" },
                        { id: "70",
                            sender: "somerandomuseridbythesender",
                            content: "How you been???" },
                    ]
                },
            ],
        };
    },
    components: { MessagePreviews }
}
</script>


<template>
    <div>
        <div v-for="msg in messages" @click="currentSelected = msg.id">
            <MessagePreviews :msgs="msg.messages" :sender="msg.messages[0].sender" :id="msg.id" :selected="this.currentSelected" />
        </div>
    </div>


</template>

<style>
    ::-webkit-scrollbar {
  width: 7px;
}

/* Track */
::-webkit-scrollbar-track {
  background: transparent; 
}
 
/* Handle */
::-webkit-scrollbar-thumb {
  background: #888; 
}

/* Handle on hover */
::-webkit-scrollbar-thumb:hover {
  background: #555; 
}

</style>
