<template>
    <div class="banner">
        <div  @click="openUrl(url1)" class="ctrl-box">
            <a :href="url" target="_blank"> 
                <img src="../assets/images/1.jpg" alt="" class="img-fluid rounded"/>
            </a>
            <div  @click="openUrl(url1)" class="box">
                <a class="label"
                href="https://bd.juejin.cn?utm_campaign=bd&amp;utm_source=web&amp;utm_medium=banner"
                target="_blank">
                <span class="inco">投放</span> <span>广告</span></a
                >
            </div>
        </div>
        <div @click="openUrl(url1)" class="ctrl-box">
            <a :href="url" target="_blank"> 
                <img src="../assets/images/2.jpg" alt="" class="img-fluid rounded"/>
            <div @click="openUrl(url1)" class="box">
                <a class="label" target="_blank">
                <span class="inco">投放</span> <span>广告</span>
                </a>
            </div>
            </a>
            
        </div>
    </div>
</template>

<script>
export default{
    methods:{
            // function(){
            //  let ctrlBox=document.getElementsByClassName("ctrl-box")[0]
            //     let img= ctrlBox.getElementsByTagName("img")[0]
            //     console.log(img)   
            // }
            // divHandle(){
            //     console.log("1")
            // },
            openUrl(){
                window.location.href=this.url1
            },
    },
    data(){
        return{
            url1:"https://bd.juejin.cn?utm_campaign=bd&amp;utm_source=web&amp;utm_medium=banner",
        }
        
    }
}
</script>


<style>
.ctrl-box{
    cursor: pointer;
}
.banner .img-fluid{
    margin-bottom: 10px;
}
.banner .box .label span{
    vertical-align: top;
}
.box .inco{
    display: none;
}
.box{
    position: relative;
}
.box span{
    /* position: relative;
    left: 180px;
    bottom: 40px;
    line-height: 18px;
    height: 18px;
    font-size: 10px;
    z-index: 1;
    transform: scale(0.5);
    transform-origin: right bottom;
    color: #fff;
    background-color: rgba(0, 0, 0, 0.2);
    border: 1px solid #fff;
    border-radius: 6px;
    padding-left: 5px;
    padding-right: 5px;
    font-weight: 300; */
    position: absolute;
    right: 10px;
    bottom: 10px;
    line-height: 36px;
    height: 36px;
    font-size: 20px;
    z-index: 100;
    transform: scale(.5);
    -webkit-transform: scale(.5);
    transform-origin: right bottom;
    -webkit-transform-origin: right bottom;
    color: #fff;
    background-color: rgba(0,0,0,.2);
    border: 1px solid #fff;
    border-radius: 6px;
    padding-left: 15px;
    padding-right: 15px;
    font-weight: 300
}
</style>
