<template>
    <header class="flex flex-col justify-start	" style="overflow-y: auto;overflow-x: hidden;">
        <horizontalHeaderSectionLogo />
        <horizontalHeaderButton to="/home" name="Home" :notification="notify['Home']" />
        <horizontalHeaderSectionTitle title="account" />
        <horizontalHeaderButton to="/profile" name="Profile" :notification="notify['Profile']" />
        <horizontalHeaderButton to="/favourite" name="Favourite" :notification="notify['Favourite']" />
        <horizontalHeaderButton to="/chats" name="Chats" :notification="notify['Chats']" />
        <horizontalHeaderButton to="/friends" name="Friends" :notification="notify['Friends']" />
        <horizontalHeaderButton to="/wallet" name="Wallet" :notification="notify['Wallet']" />
        <horizontalHeaderSectionTitle title="main" />
        <horizontalHeaderButton to="/store" name="Store" isActive="true" :notification="notify['Store']" />
        <horizontalHeaderButton to="/market" name="market" :notification="notify['market']" />
        <horizontalHeaderButton to="/streams" name="Streams" :notification="notify['Streams']" />
        <horizontalHeaderButton to="/community" name="Community" :notification="notify['Community']" />
        <horizontalHeaderSectionTitle title="support" />
        <horizontalHeaderButton to="/report" name="Report" :notification="notify['Report']" />
        <horizontalHeaderButton to="/help" name="Help" :notification="notify['Help']" />
    </header>
</template>

<style>
header {
    width: 242px;
    background-color: var(--light4);
    height: 100vh;
    border-right: 1px solid #f2f2f2;
}
</style>
<script>
export default {
    data() {
        return {
            notify: { Favourite: 12 }
        }
    }
}
</script>