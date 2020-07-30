<template>
<div id="nav">
    <div class="nav-left">
        <h1>头条</h1>
        <section class="nav-list">
            <section v-for="(item,index) in navlist" :key="index" class="nav-list-sec">
                {{item.text}}
            </section>
        </section>
    </div>
    <div class="nav-middle">中间</div>
    <div class="nav-right">右边</div>
</div>
</template>

<script>

export default {
//import引入的组件需要注入到对象中才能使用
components: {},
data() {
//这里存放数据
return {
    navlist:[
        {id:1,text:"推荐"},
        {id:2,text:"西瓜视频"},
        {id:3,text:"财经"},
        {id:4,text:"热点"},
        {id:5,text:"直播"},
        {id:6,text:"图片"},
        {id:7,text:"科技"},
        {id:8,text:"娱乐"},
        {id:9,text:"游戏"},
        {id:10,text:"体育"},
        {id:11,text:"懂车帝"},
        {id:12,text:"热点"},
        
    
    ]
};
},
//监听属性 类似于data概念
computed: {},
//监控data中的数据变化
watch: {},
//方法集合
methods: {

},
//生命周期 - 创建完成（可以访问当前this实例）
created() {

},
//生命周期 - 挂载完成（可以访问DOM元素）
mounted() {

},
beforeCreate() {}, //生命周期 - 创建之前
beforeMount() {}, //生命周期 - 挂载之前
beforeUpdate() {}, //生命周期 - 更新之前
updated() {}, //生命周期 - 更新之后
beforeDestroy() {}, //生命周期 - 销毁之前
destroyed() {}, //生命周期 - 销毁完成
activated() {}, //如果页面有keep-alive缓存功能，这个函数会触发
}
</script>
<style lang= "less" scoped>
#nav {
    width: 80vw;
    margin: 0 10vw;
    display: flex;
  .nav-left {
      flex: 1;
      text-align: center;
      font-weight: 100;
      color: red;
      .nav-list{
          section{
              width: 100%;
              height: 30px;
              text-align: center;
              line-height: 30px;
              transition: all .3s;
              color: black;
              &:hover{
                  background: red;
                  border-radius: 5px;
                  color: white;
                  cursor: pointer;
              }
          }
      }
  }

  .nav-middle {
      flex: 3;
  }

  .nav-right {
      flex: 2;
  }
}
</style>