<template>
    <div class="apps">
        <!--<div  class="app2">-->
        <button class="app7"><router-link to="/ownPage/weibos" class="ys">取消</router-link></button>
        <div class="zhuanfa">转发圈子</div>
        <button class="fasong">发送</button>
        <span class="xian"></span>
        <!--</div>-->
        <mu-text-field class="pinglun"   v-model="value9" placeholder="写评论。。。" multi-line :rows="3" :rows-max="6"></mu-text-field>
        <input class="kuang" type="checkbox" />
        <ul class="ziti">
            <span>同时转发</span></ul>
        <div class="app-bottom">
            <div class="kongbai">
                <span></span>
                <button  class="zhaopian" ><img src="../../../assets/img/图层 4.png" /></button>
                <button  class="biaoqing" ><img src="../../../assets/img/图层 5.png" /></button>
            </div>
        </div>
    </div>
</template>
<script>
    export default {

        name:"Forwaid"

    }
</script>
<style scoped lang="scss">
    .apps{
        background: #ffffff;
    }
    .app1 {
        width: 6.4rem;
        height: 40px;
        background-color: #ffffff;
        text-align:center;
    }
    .app7 {
        float: left;
        margin: 0;
        padding: 0;
        border: 1px solid transparent;
        background:none;
        position: absolute;
        left: 10px;
        top: 32px;
        color: #333333;
    }
    .zhuanfa {
        height: 29px;
        font-size: 20px;
        float:left;
        position: absolute;
        left: 50%;
        top: 30px;
        margin-left: -10%;
        line-height: 26px;
        color: #333333;
    }
    .fasong{
        margin: 0;
        padding: 0;
        background:none;
        color: #999999;
        float: right;
        position: absolute;
        right: 3%;
        top: 30px;
        width: 13%;
        border-radius: 5px;
        border: solid 1px #999999;
    }
    .pinglun{
        border:none;
        position: absolute;
        top: 80px;
        left: 10px;
        background:none;
    }
    .app-bottom{
        position: fixed;
        bottom: 0;
        left:0;
    }
    .kongbai{
        width: 6.4rem;
        height: 50px;
        background:none;
        border-top: 1px solid #cccccc;

    }
    .xian {
        width: 6.4rem;
        height: 1px;
        background-color: #dddddd;
        position: absolute;
        top: 70px;
        content: '';
        border-bottom: 1px solid #cccccc;
        transform-origin: 0 100%;
        transform: scaleY(.5);
    }
    .zhaopian {
        background: white;
        position: absolute;
        left: 10%;
        top: 15px;
        margin: 0;
        padding: 0;
        border: 1px solid transparent;
        float: left;
        height: 25px;
        width: 25px;
    }
    .biaoqing{
        margin: 0;
        padding: 0;
        background: white;
        border: 1px solid transparent;
        float: left;
        position: relative;
        left: 30%;
        top: 15px;
        height: 25px;
        width: 25px;
    }
    .kuang{
        position: absolute;
        left: 2%;
        bottom: 55px;
    }
    .ziti{
        font-size: 15px;
        letter-spacing: 0px;
        color: #999999;
        position: absolute;
        left: 7%;
        bottom: 48px;
        margin: 0;
        padding: 0;
    }
    .ys{
        color: #333333;
    }
</style>
<style scoped lang="scss">

</style>
