<template>
    <header class="flex flex-col justify-start	">
        <horizontalHeaderSectionLogo />
        <horizontalHeaderButton to="/home" name="Profile" notification="120" isActive=true />
        <horizontalHeaderSectionTitle title="ciao" />
        <horizontalHeaderButton to="/hodme" name="Favourite" notification="2" />
        <horizontalHeaderButton to="/hodme" name="dsa"  />
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
