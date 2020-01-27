<template>
    <div>
        <button id="sign-in"><img src="~assets/icons/signin.png" />Sign In</button>
        <button id="sign-up"><img src="~assets/icons/signup.png" />Sign Up</button>
    </div>
</template>

<style lang="scss" scoped>
    button {
        height: 65px;
        width: 50px;
        border: none;
        padding-top: 35px;
        font-size: 10px;
        vertical-align: middle;
        text-align: center;
        font-weight: bold;
        position: relative;
        img {
            width: 30px;
            height: 30px;
            position: absolute;
            left: 10px;
            top: 10px;
        }
    }
    #sign-up {
        background: #63cf0d;
    }
    #sign-in {
        background: #E49349;
    }
</style>