<template>
    <nav>
        <ul id="left-nav">
            <li><a>News</a></li>
            <li><a>Cards</a></li>
            <li><a>Decks</a></li>
            <li><a>Mechanics</a>
                <ul class="sub">
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
            <li><SearchBox /></li>
            <li><Themer /></li>
            <li><SignIn /></li>
        </ul>
    </nav>
</template>

<script>
import SearchBox from '~/components/SearchBox.vue';
import SignIn from '~/components/SignIn.vue';
import Themer from '~/components/Themer.vue';

export default {
  components: {
    SearchBox,
    SignIn,
    Themer,
  }
}
</script>

<style lang="scss" scoped>

nav {
    position: fixed;
    top: 0px;
    left: 0px;
    width: 100%;
    height: 65px;
    padding: 0px 15%;
    background: #111111;
    ul {
        list-style-type: none;
        height: 100%;
        display: inline-block;
        vertical-align: middle;
        padding: 20px 0;
        color: #338de4;
        font-size: 16px;
        li {
            display: inline-block;
            vertical-align: middle;
            text-align: center;
            padding: 0px 20px;
            font-weight: bold;
            position: relative;
            sub.ul {
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
    padding: 0;
}

</style>