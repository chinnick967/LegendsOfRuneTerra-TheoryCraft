<template>
    <div style="position: relative; margin-right: 10px;">
        <input type="text" placeholder="Cards, keywords, decks, etc." />
        <button><img class="search-icon" src="~assets/icons/magnify2.png" /></button>
    </div>
</template>

<style lang="scss" scoped>
    input {
        transform: skew(-0.15rad);
        border-radius: 4px;
        border: 1px solid #ccc;
        padding: 8px 20px;
        padding-right: 35px;
        width: 240px;
        &:focus {
            border-color: #338de4;
        }
    }
    button {
        background-color:#338de4;
        width: 28px;
        height: 28px;
        transform: skew(-0.15rad);
        position: absolute;
        top: 3px;
        right: 3px;
        outline: none;
        border: none;
        font-family: $mainFont;
    }
    .search-icon {
        width: 21px;
        height: 21px;
        transform: skew(0.15rad);
        position: relative;
        top: 1px;
        left: -2px;
        pointer-events: none;
    }
</style>