<template>

    <div class="filterOption">
        <div>
            <span>{{ subName }}<b>{{ name }}</b></span>
            <div class="arrow-up"></div>
        </div>
    </div>
</template>
<style>
.filterOption {
    padding: 6px;
    border-radius: 15px;
    background-color: var(--light2);
    width: fit-content;
    color: #5F5F5F;
}

.filterOption div {
    display: flex;
    flex-direction: row;
    align-items: center;
}

.filterOption div span {
    margin-left: 15px;
}

.arrow-up {
    width: 0;
    height: 0;
    border-left: 8px solid transparent;
    border-right: 8px solid transparent;

    border-bottom: 8px solid #5F5F5F;
    transition: all 0.5s;
    margin-left: 6px;
    margin-right: 10px;
    font-style: normal;
    font-weight: 400;
    font-size: 14px;
    line-height: 19px;

    transform: rotateZ(180deg);
}
</style>
<script>
export default {
    props: {
        subName: String,
        name: String,
    }
}
</script>
