<template>
    <div class="blog">
        <div id="center1">
            <img src="./component/img/返回.png" alt="" @click="back" class="img-left">
            <span class="center">圈子正文</span>
            <img src="./component/img/daohang.png" alt="" class="img-right">
        </div>
        <div id="center2">
            <ul>
            <li>
                <div class="detail-content">
                    <router-link to="/ownPage/weibos">
                        <img src="../../assets/img/mood (1).jpg" alt="" class="head-por">
                    </router-link>

                    <div class="con-name">
                        <div class="name-id">杂交水稻研究人</div>
                        <div class="name-time">1小时前</div>
                    </div>
                </div>

                <div class="text">

            <span>
              【河南夏邑借棚改之名强征千亩耕地 农业局称：土地权证发错了！】村里的一位老党员称，9月2日，乡政府组织村里开过一次村民代表大会，说的重点是棚户区改造的情况，当时乡党委书记董天成在会上明确表示，土地批文下来后才会征地。没想到会后第二天，就把耕地全部铲平了。
            </span>

                </div>
                <div class="image">
                    <img src="../../assets/img/mood (1).jpg" alt="">
                    <img src="../../assets/img/mood (2).jpg" alt="">
                    <img src="../../assets/img/mood (3).jpg" alt="">
                </div>
            </li>
            </ul>
        </div>
        <div>
            <div id="container-span">
                <span @click="jump">转发109</span>
                <span @click="jump1">评论8989</span>
                <span @click="jump2">点赞908</span>
            </div>
            <router-view></router-view>
        </div>
        <div id="center5">
            <Wrapper1></Wrapper1>
        </div>
    </div>
</template>

<script>
    import Wrapper1 from '@/views/blog/component/Wrapper1.vue';
    import Content from '@/views/blog/component/Content.vue';

    export default {
        components: {
            Wrapper1,Content
        },
        methods:{
            back(){
                this.$router.push('/blog/details');
            },
            jump(){
                this.$router.push('/blog/passage');
            },
            jump1(){
                this.$router.push('/blog/passage/commentwb');
            },
            jump2(){
                this.$router.push('/blog/passage/likeweibo');
            }
        }
    }
</script>

<style scoped lang="scss">
.blog{
    background: #e5e5e5;
}
#center1{
    background: white;
    height: 1rem;
    display: flex;
    line-height: 1rem;
    margin-bottom: 0.3rem;
    img{
        width: 0.5rem;
        height: 0.5rem;
        margin-top: 0.25rem;
    }
    & .img-left{
        margin-left: 0.15rem;
    }
    & .center{
         text-align: center;
        flex: 1;
     }
    & .img-right{
        margin-right: 0.3rem;
    }
}
#center2{
    background: white;
    padding: 0.2rem;
}
.detail{
    margin-top: .2rem;
}
.detail-content{
    height: 78px;
    img{
        float:left;
    }
    & .con-name{
        width: 326px;
        font-size: 20px;
        color: #2196f3;
        & .name-time{
            font-size: 16px;
            color:rgb(149,149,147);
        }
    }
}
.detail li{
    width: 100%;
    padding-left: .4rem;
    padding-right: .4rem;
    margin-top: .2rem;
    background: white;
}
.head-por{
    width: 1.3rem;
    height: 1.3rem;
    margin-right: .2rem;
}
.name{
    display: inline-block;
}
.name .name-id{
    color: #2196f3;
    font-size: .5rem;
}
.image{
    width: 100%;
}
.image img{
    width: 1.7rem;
    height: 1.7rem;
    margin-right: .16rem;
}
#container-span{
    background: white;
    height: .8rem;
}
#container-span span{
    height :100%;
    line-height: .8rem;
    color: gray;
    font-weight: 200;
    margin: auto 10px;
}
#container-span span:hover{
    color:blue;
    border-bottom: 1px solid blue;
}
#report{
    width: 100%;
    padding-left: .4rem;
    padding-right: .4rem;
    margin-top: .2rem;
    background: white;
}
#report img{
    float: left;
    width: 1rem;
    height: 1rem;

}
#report span{
    font-size: xx-small;
}
#report .name-id{
    font-size: 5px;
    color: blue;
}
#report .name-time{
    font-size: 5px;
    margin-top:.2rem ;
}
#report .reportt{
    border-bottom: 1px solid gainsboro;
    margin-bottom: .1rem;
}
</style>