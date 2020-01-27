<template>
    <div id="HomeMenu">
        <ul>
            <li><img src="~assets/icons/intro.png" /></li>
            <li><img src="~assets/icons/news.png" /></li>
            <li><img src="~assets/icons/analytics.png" /></li>
            <li><img src="~assets/icons/cards.png" /></li>
            <li><img src="~assets/icons/strategy.png" /></li>
        </ul>
    </div>
</template>

<style lang="scss" scoped>
    #HomeMenu {
        position: fixed;
        margin: 0 auto;
        bottom: 0;
        width:  600px;
        height: 75px;
        background: black;
        color: white;
        &:before {
            content: '';
            position: absolute;
            left: -70px;
            top: 0px;
            width: 0;
            height: 0;
            border-bottom: 100px solid black;
            border-left: 70px solid transparent;
        }
        &:after {
            content: '';
            position: absolute;
            right: -70px;
            top: 0px;
            width: 0;
            height: 0;
            border-bottom: 100px solid black;
            border-right: 70px solid transparent;
        }
    }
    ul {
        text-align: center;
        li {
            display: inline-block;
            height: 60px;
            width: 60px;
            vertical-align: top;
            background: #338de4;
            img {
                width: 50px;
                height: 50px;
            }
        }
    }
</style>