<template>
    <nav>
        <ul id="left-nav">
            <li><a>News</a></li>
            <li><a>Cards</a></li>
            <li><a>Decks</a></li>
            <li><a>Mechanics</a>
                <ul>
                    <li><a>Regions</a></li>
                    <li><a>Keywords</a></li>
                    <li><a>Level Up</a></li>
                    <li><a>Champions</a></li>
                    <li><a>Followers</a></li>
                    <li><a>Spells</a></li>
                </ul>
            </li>
            <li><a>Guides</a></li>
            <li><a>Live Streams</a></li>
        </ul>
        <ul id="right-nav">
            <li><input type="text" placeholder="Cards, keywords, decks, etc." /></li>
            <li><button>Sign In</button></li>
        </ul>
    </nav>
</template>

<style lang="scss" scoped>

nav {
    position: fixed;
    top: 0px;
    left: 0px;
    width: 100%;
    height: 100px;
    padding: 25px 20%;
    ul {
        list-style-type: none;
        height: 100%;
        display: inline-block;
        vertical-align: middle;
        padding: 15px 0;
        color: #35495e;
        font-size: 16px;
        li {
            display: inline-block;
            vertical-align: middle;
            text-align: center;
            padding: 0px 20px;
            font-weight: bold;
            position: relative;
            ul {
                position: absolute;
                display: block;
                top: 25px;
                left: 0px;
                max-height: 0px;
                height: auto;
                overflow: hidden;
                padding: 0;
                color: black;
                background: #eee;
                font-size: 14px;
                li {
                    margin: 5px 0;
                }
                &:hover {
                    max-height: 600px;
                }
            }
            &:hover {
                cursor: pointer;
                ul {
                    transition: max-height 500ms ease-in-out;
                    max-height: 600px;
                    padding: 10px;
                }
            }
        }
    }
}

#left-nav {
    float: left;
    width: 650px;
}

#right-nav {
    float: right;
}

</style>