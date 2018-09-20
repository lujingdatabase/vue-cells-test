<template>
  <div id="app">
     <Collapse v-model="value">
        <Panel name="1">
            多图轮播：
            <p slot="content">
                    <j-mult-slider    :staticData ='datass' nameCor='#000' unitCor='#000' exCor='#000' valCor='#000' ></j-mult-slider>

            </p>
        </Panel>
        <Panel name="2">
           色块图：
            <p slot="content">
                 <j-color-block totalNum=250 titleColor='#000' width=500 height=200 :staticData='dataofcolorblock'></j-color-block>
            </p>
        </Panel>
        <Panel name="3">
            待补充
            <p slot="content">。。。</p>
        </Panel>
        <Panel name="4">
            待补充
            <p slot="content">。。。</p>
        </Panel>
    </Collapse>
    
   
    
    
  </div>
</template>

<script>
export default {
  name: 'app',
  data () {
    return {
      value:'1',
      msg: 'Welcome to Your Vue.js App',
      dataofcolorblock:[{
                totavaluelNum: 8, //总值
                valueNum: 4, //当前值
                titlename: '测试标题',
            }],
      datass:[{
                    img: "https://www.baidu.com/img/bd_logo1.png",
                    ex: "第",
                    x: 1,
                    unit: "家",
                    y: "超市"
                },
                {
                    img: "https://www.baidu.com/img/bd_logo1.png",
                    ex: "第",
                    x: 2,
                    unit: "家",
                    y: "超市"
                },
                {
                    img: "https://www.baidu.com/img/bd_logo1.png",
                    ex: "第",
                    x: 3,
                    unit: "家",
                    y: "超市"
                }]
    }
  }
}
</script>

<style>
#app {
  /* font-family: 'Avenir', Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #2c3e50;
  margin-top: 60px; */
}

/* h1, h2 {
  font-weight: normal;
}

ul {
  list-style-type: none;
  padding: 0;
}

li {
  display: inline-block;
  margin: 0 10px;
}

a {
  color: #42b983;
} */
</style>
