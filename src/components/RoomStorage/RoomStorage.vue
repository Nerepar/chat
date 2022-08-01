<template src="./template.html"/>

<script>
    import ChatRoomRegistry from "@/components/ChatRoomRegistry/ChatRoomRegistry";

    export default {
        name: "RoomStorage",
        components: {ChatRoomRegistry},
        methods: {
            addRoomClick() {
                this.$emit('addRoomClick');
            }
        }
    }
</script>

<style scoped src="./style.less" lang="less">

</style>