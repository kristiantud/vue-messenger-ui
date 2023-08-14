

<template>
    <div style="height: 700px; width: 1300px; background-color: #202020;  margin: auto; margin-top: 50px; border-radius: 10px; display: flex;">
        <div style="overflow: auto; width: 600px;">
            <MsgPreviewWidget />
        </div>
        <div style="width: 100%;">
            <MsgLogsWidget />
        </div>
    </div>


</template>


<script>
    import MsgLogsWidget from './MsgLogsWidget.vue';
import MsgPreviewWidget from './MsgPreviewWidget.vue';

    export default {
        components: {
    MsgPreviewWidget,
    MsgLogsWidget
}
    }
</script>

