

<!-- will have an array of messages that this loops through -->
<!-- will populate the MsgPrev section of the messageswidget -->

<script>
import MessagePreviews from './MessagePreviews.vue';

    export default {
    name: 'MsgPreviewWidget',
    data: function () {
        return {
            messages: [
                {
                    id: "1",
                    messages: [
                        { id: "69",
                            sender: "somerandomuseridbythesender",
                            content: "Hello brother!" },
                        { id: "70",
                            sender: "somerandomuseridbythesender",
                            content: "How you been???" },
                    ]
                },
                {
                    id: "2",
                    messages: [
                        { id: "69",
                            sender: "somerandomuseridbythesender",
                            content: "Hello brother!" },
                        { id: "70",
                            sender: "somerandomuseridbythesender",
                            content: "How you been???" },
                    ]
                },
                {
                    id: "3",
                    messages: [
                        { id: "69",
                            sender: "somerandomuseridbythesender",
                            content: "Hello brother!" },
                        { id: "70",
                            sender: "somerandomuseridbythesender",
                            content: "How you been???" },
                    ]
                },
                {
                    id: "4",
                    messages: [
                        { id: "69",
                            sender: "somerandomuseridbythesender",
                            content: "Hello brother!" },
                        { id: "70",
                            sender: "somerandomuseridbythesender",
                            content: "How you been???" },
                    ]
                },
                {
                    id: "5",
                    messages: [
                        { id: "69",
                            sender: "somerandomuseridbythesender",
                            content: "Hello brother!" },
                        { id: "70",
                            sender: "somerandomuseridbythesender",
                            content: "How you been???" },
                    ]
                },
                {
                    id: "6",
                    messages: [
                        { id: "69",
                            sender: "somerandomuseridbythesender",
                            content: "Hello brother!" },
                        { id: "70",
                            sender: "somerandomuseridbythesender",
                            content: "How you been???" },
                    ]
                },
                {
                    id: "7",
                    messages: [
                        { id: "69",
                            sender: "somerandomuseridbythesender",
                            content: "Hello brother!" },
                        { id: "70",
                            sender: "somerandomuseridbythesender",
                            content: "How you been???" },
                    ]
                },
            ]
        };
    },
    components: { MessagePreviews }
}
</script>


<template>
    <div>
        <div v-for="msg in messages">
            <MessagePreviews :msgs="msg.messages" :sender="msg.messages[0].sender"  />
        </div>
    </div>


</template>

