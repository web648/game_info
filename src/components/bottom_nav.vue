<template>
    <div class="nav_list">
        <slot>
            <ul class="nav_fixed">
                <router-link to="/" tag="li" exact class="icon icon_home" style="color:#f60;">主页</router-link>
                <router-link to="personalLetter" tag="li" class="icon icon_personalLetter">私信 <i class="ico_num"></i></router-link>
                <router-link to="toFind" tag="li" class="icon icon_finder">发现</router-link>
                <router-link to="user" tag="li" class="icon icon_me">我</router-link>
            </ul>
        </slot>
    </div>
</template>

<script>
    export default{
        data (){
            return{

            }
        },
        methods:{

        }
    }
</script>

<style scoped lang="less">
.nav_list{
    // overflow: hidden;
    .nav_fixed{
        display: flex;
        width: 100%;
        background: #fff;
        border-top: 1px solid #e5e5e5;
        padding-top: .15rem;
        position: fixed;
        bottom: 0;
        left: 0;
        li{
            flex: 1;
            justify-content: center;
            text-align: center;
            cursor: pointer;
            overflow: hidden;
            padding-bottom: 0.1rem;
            i{
                display: block;
                color: #fff;
                width: .12rem;
                height: .12rem;
                border-radius: 50%;
                background: red;
                position: absolute;
                top: .1rem;
                right: 35%;
            }
        }
    }
}
</style>

