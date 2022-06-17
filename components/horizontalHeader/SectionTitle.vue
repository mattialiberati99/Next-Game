<template>
    <h2 class="SectionTitle">{{ title }}</h2>
</template>
<style>
.SectionTitle {
    width: 100%;
    text-transform: uppercase;
    margin-left: 30px;
    margin-top: 24px;
    margin-bottom: 21px;
    font-weight: 700;
    font-size: 12px;
    line-height: 16px;
    color: #767676;
}
</style>
<script>
export default {
    props: {
        title: String
    }
}
</script>