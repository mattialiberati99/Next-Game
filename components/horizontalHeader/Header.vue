<template>
    <header class="flex flex-col justify-start	">
        <horizontalHeaderSectionLogo />
        <horizontalHeaderButton to="/home" name="Home" />
        <horizontalHeaderSectionTitle title="account" />
        <horizontalHeaderButton to="/profile" name="Profile" />
        <horizontalHeaderButton to="/favourite" name="Favourite" notification="15" />
        <horizontalHeaderButton to="/chat" name="Chat" />
        <horizontalHeaderButton to="/friends" name="Friends" />
        <horizontalHeaderButton to="/wallet" name="Wallet" />
        <horizontalHeaderSectionTitle title="main" />
        <horizontalHeaderButton to="/store" name="Store" isActive="true" />
        <horizontalHeaderButton to="/market" name="market" />
        <horizontalHeaderButton to="/streams" name="Streams" />
        <horizontalHeaderButton to="/community" name="Community" />
        <horizontalHeaderSectionTitle title="support" />
        <horizontalHeaderButton to="/report" name="Report" />
        <horizontalHeaderButton to="/help" name="Help" />
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
