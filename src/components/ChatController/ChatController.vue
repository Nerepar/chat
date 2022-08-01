<template src="./template.html"/>

<script>
    import ChatAddRoom from "@/components/ChatAddRoom/ChatAddRoom";
    import ChatRoom from "@/components/ChatRoom/ChatRoom";
    import RoomStorage from "@/components/RoomStorage/RoomStorage";

    export default {
        name: "ChatController",
        components: {
            ChatAddRoom, ChatRoom, RoomStorage
        },
        data() {
            return {
                addFormVisible: false,
                indexRoom: 0,
                desk: {
                    title: 'Комнаты',
                    rooms: []
                },
            };
        },
        methods: {
            addRoomClick() {
                this.addFormVisible = true
            },
            closeAddRoom() {
                this.addFormVisible = false
            },
            addRoom(roomData) {
                this.indexRoom++;
                this.desk[0].rooms.push(roomData)
            }
        }
    }
</script>

<style scoped src="./style.less" lang="less">

</style>