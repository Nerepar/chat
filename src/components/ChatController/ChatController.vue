<template src="./template.html"/>

<script>
    import ChatAddRoom from "@/components/ChatAddRoom/ChatAddRoom";
    import ChatRoom from "@/components/ChatRoom/ChatRoom";
    import ChatRoomRegistry from "@/components/ChatRoomRegistry/ChatRoomRegistry";

    export default {
        name: "ChatController",
        components: {
            ChatAddRoom, ChatRoom, ChatRoomRegistry
        },
        data() {
            return {

            }
        }
    }
</script>

<style scoped src="./style.less" lang="less">

</style>