<template>
  <div id="firstdiv">
    <header>
      <div>

      </div> 
    </header>
    <br/>
    <span style="display:inline-block;border-top:1px solid;width:46%;height:.5em;color:#ccc;"></span>
    <span style="display:inline-block;width:6%;height:.5em;"></span>
    <span style="display:inline-block;border-top:1px solid;width:46%;height:.5em;color:#ccc;"></span>
    <br/>
    <br/>
    <div id="first-container">
      <div id="first-menu">
        <router-link :to="'/three'">
          <div class="first-small-place">
            <h2>创意小角落</h2>
          </div>
        </router-link>
        <router-link :to="'/second'">
          <div class="first-small-flower">
            <h2>温馨小花园</h2>
          </div>
        </router-link>
        <router-link :to="'/second'">
          <div class="first-small-sweet">
            <h2>甜美小点心</h2>
          </div>
        </router-link>
        <router-link :to="'/second'">
          <div class="first-small-message">
            <h2>信息统计表</h2>
          </div>
        </router-link>
      </div>
    </div>
    <br/>
    <span style="display:inline-block;border-top:1px solid;width:45%;height:.5em;color:#ccc;"></span>
    <span style="display:inline-block;width:8%;height:.5em;"></span>
    <span style="display:inline-block;border-top:1px solid;width:45%;height:.5em;color:#ccc;"></span>
    <br/>
    <br/>
    <div id="first-content">
      <div style="height:295px;">
        <div class="body-div">
          <img src="/static/images/t1.jpg"/>
          <div class="first-pointers bgwh onept"></div>
        </div>
        <div class="body-div">
          <div class="bd-firstmsg">
            <div class="first-title">你好呀</div>
            <h3>第二标题</h3>
            <div>描述</div>
          </div>
          <div class="bd-secondmsg">
            <div class="first-title first-title-left">你好呀</div>
            <h3>第二标题</h3>
            <div class="right-ms">描述</div>
          </div>
          <div class="first-pointers onet"></div>
          <div class="first-pointers onew"></div>
        </div>
        <div class="body-div">
          <img src="/static/images/t2.jpg"/>
          <div class="first-pointers bgwh lastpt"></div>
        </div>
        <div class="body-div">
          <img src="/static/images/t3.jpg"/>
          <div class="first-pointers bgwh first-th-a hidden"></div>
        </div>
        <div class="body-div three-screen">
          <div class="one-msg one-msg-top three-screen-div">
            <div class="first-title">你好呀</div>
            <h3>第二标题</h3>
            <div>描述</div>
          </div>
          <div hidden class="first-pointers first-th-b hidden"></div>
        </div>
      </div>

      <div>

        <div class="body-div second-onept">
          <div class="one-msg one-msg-bottom second-onemsg">
            <div class="first-title first-title-left">你好呀</div>
            <h3>第二标题</h3>
            <div class="right-ms">描述</div>
          </div>
          <div class="first-pointers hidden second-th-a"></div>
        </div>

        <div class="body-div second-twpt">
          <img src="/static/images/t4.jpg"/>
          <div class="first-pointers bgwh hidden second-th-b"></div>
        </div>

        <div class="body-div second-as">
          <img src="/static/images/t5.jpg"/>
          <div class="first-pointers bgwh onept"></div>
        </div>

        <div class="body-div second-lasmsg">
          <div class="bd-firstmsg">
            <div class="first-title">你好呀</div>
            <h3>第二标题</h3>
            <div>描述</div>
          </div>
          
          <div class="bd-secondmsg">
            <div class="first-title first-title-left">你好呀</div>
            <h3>第二标题</h3>
            <div class="right-ms">描述</div>
          </div>
          <div class="first-pointers onet"></div>
          <div class="first-pointers onew"></div>

        </div>

        <div class="body-div second-laspt">
          <img src="/static/images/t6.jpg"/>
          <div class="first-pointers bgwh lastpt"></div>
        </div>

      </div>
    </div>

    <footer></footer>  
  </div>
</template>

<script>
    export default {
        name: "first",
        created() {
        }
    }
</script>

<style>
a {
  text-decoration: none;
}
body {
  overflow-x: hidden !important;
}
#firstdiv {
  
  height: 100%;
  background-repeat: no-repeat; 
}
header {
  width: 100%;
  height: 30em;
  background-image: url(".././assets/jks.jpg");
  background-repeat: no-repeat; 
  background-size: 100%;
}
#first-menu {
  width:100%;
  margin:0 auto;
}
#first-container {
  width: 100%;
  margin: 0 auto;
}
/* VVV颈部四个导航菜单样式VVV */
.first-th-a {
  top:-220px;
  left:282px;
}
.first-th-b {
  top:-218px;
  left:-7px;
  z-index:9;
}
.second-th-a {
  top:-90px;
  left:283px;
  z-index:9;
}
.second-th-b {
  top:-92px;
  right:10px;
}
.first-small-message {
  background-image: url("/static/images/msg.jpg");
}
.first-small-flower {
  background-image: url("/static/images/flower.jpg");
}
.first-small-place {
  background-image: url("/static/images/place.jpg");
}
.first-small-sweet {
  background-image: url("/static/images/sweet.jpg");
}
.first-small-sweet,.first-small-place,.first-small-flower,.first-small-message {
  background-repeat: no-repeat; 
  background-size: 100%;
  color: white;
  display: inline-block;
  margin:0 20px 0 20px;
  width:360px;
  height: 180px;
  line-height: 150px;
}
/* ^^^颈部四个导航菜单样式 ^^^*/
/* 描述信息指向小三角 */
.first-pointers {
  position:relative;
  width:14px;
  height:14px;
  background-color:#F4F4F4F4;
  transform:rotate(45deg);
  -ms-transform:rotate(45deg); 	/* IE 9 */
  -moz-transform:rotate(45deg); 	/* Firefox */
  -webkit-transform:rotate(45deg); /* Safari 和 Chrome */
  -o-transform:rotate(45deg); 	/* Opera */
}
/* 图片丶描述容器 */
#first-content {
  margin:0 auto;
  width:1470px;
  height:600px;
  padding:0 20px 0 20px;
  overflow:hidden;
}
/* 图片格式 */
#first-content img {
  width:100%;
  height:100%;
}
/* 小模块样式 */
#first-content .body-div{
  margin-left:4px;
  width:290px;
  height:290px;
  float:left;
}
.body-div h3{
  margin:5px 20px 5px 0;
}
/* 两个描述内容小模块样式 */
.bd-firstmsg{
  padding:15px 0 0 20px;
  position:relative;
  background:#F4F4F4F4;
  width:270px;height:133px;
  margin-bottom:4px;z-index:999;
  text-align:left;
}
.onept {
  top:-232px;
  left:281px;
}
.lastpt{
  top:-87px;
  left:-9px;
}
.onet{
  top:-226px;
  left:-7px;
  z-index:9;
}
.onew{
  top:-95px;
  right:-283px;
  z-index:9;
}
.one-msg {
  position:relative;
  background:#F4F4F4F4;
  height:275px;
  margin-bottom:4px;
  z-index:999;
}
.one-msg-top{
  text-align: left;
  padding:15px 0 0 20px;
}

.one-msg-bottom{
  text-align: right;
  padding:15px 0 0 0;
}
.right-ms {
  margin:0 20px 0 0;
}
.bd-secondmsg{
  position:relative;
  z-index:100;
  background:#F4F4F4F4;
  width:100%;
  height:138px;
  text-align:right;
}
.first-title {
  width:120px;
  height:40px;
  border-bottom:1px solid #ccc;
  color:#ccc;
  font-size:30px;
  font-family:STFangsong;
}
.first-title-left {
  position:relative;
  left:150px;
  top:5px;
}
.bgwh {
  background-color:white;
  width:18px;
  height:18px;
}
footer{
  width:100%;
  height:200px;
  background: #ccc;
}
@media screen and (min-width: 1530px) and (max-width: 1640px){
  .first-small-sweet,.first-small-place,.first-small-flower,.first-small-message {
    width:320px;
  }
}
@media screen and (min-width: 1460px) and (max-width: 1529px) {
  .first-small-sweet,.first-small-place,.first-small-flower,.first-small-message {
    width:320px;
    margin: 0 10px 0 10px;
  }
  .onet{
    top:-320px;
    left:-7px;
    z-index:9;
  }
  .onew{
    top:-95px !important;
    right:-333px;
    z-index:9;
  }
  .onept {
    top:-327px;
    left:330px;
  }
  /* 图片丶描述容器 */
  #first-content {
  width:1400px;
  height:800px;
  padding:0 20px 0 20px;
  }
 
  /* 小模块样式 */
  #first-content .body-div{
    margin-left:4px;
    width:340px;
    height:380px;
    margin-top: 5px;
  }
 
  /* 两个描述内容小模块样式 */
  .bd-firstmsg{
    position:relative;
    background:#F4F4F4F4;
    width:320px;
    height:173px;
    margin-bottom:4px;
    z-index:999;
    text-align:left;
  }
  .bd-secondmsg{
    position:relative;
    z-index:100;
    background:#F4F4F4F4;
    width:100%;
    height:188px;
    text-align:right;
  }
  
  .first-title-left {
    left:200px;
  }
  /* 第一排最后一个描述样式 */
  .three-screen {
    float: none;
    clear: both;
    height:150px !important;
    position:relative;
    top:-170px;
    left:1032px;
    color:#c0c0c0;
  }
  .three-screen-div {
    height:100% !important; 
    background-color:rgba(0,0,0,.4);
  }
  .hidden {
    display: none !important;
  }
  .second-onemsg{
    background: rgba(0, 0, 0, .4);
    color: #c0c0c0;
    position:relative;
    top:215px;
    height:150px;
    
  }
  .second-onept {
    position:relative;
    left:-344px;
  }
  .second-twpt {
    position:relative;
    left:-688px;
  }
  .second-laspt {
    position:relative;
    top:-385px;
    left:689px;
  }
  .second-lasmsg {
    position:relative;
    left:688px;
    top:-385px;
  }
  .second-as {
    position:relative;
    left:-688px;
  }
}
@media screen and (min-width: 1270px) and (max-width: 1459px) {
  .first-small-sweet,.first-small-place,.first-small-flower,.first-small-message {
    width:280px;
    margin: 0 10px 0 10px;
  }
  .onet{
    top:-230px;
    left:-7px;
    z-index:9;
  }
  .onew{
    top:-95px !important;
    right:-293px;
    z-index:9;
  }
  .onept {
    top:-236px;
    left:290px;
  }
  /* 图片丶描述容器 */
  #first-content {
  width:1280px;
  height:620px;
  padding:0 20px 0 80px;
  }
 
  /* 小模块样式 */
  #first-content .body-div{
    margin-left:4px;
    width:300px;
    height:300px;
    margin-top: 5px;
  }
 
  /* 两个描述内容小模块样式 */
  .bd-firstmsg{
    position:relative;
    background:#F4F4F4F4;
    width:280px;
    height:133px;
    margin-bottom:4px;
    z-index:999;
    text-align:left;
  }
  .bd-secondmsg{
    position:relative;
    z-index:100;
    background:#F4F4F4F4;
    width:100%;
    height:148px;
    text-align:right;
  }
  
  .first-title-left {
    left:160px;
  }
  /* 第一排最后一个描述样式 */
  .three-screen {
    float: none;
    clear: both;
    height:115px !important;
    position:relative;
    top:-135px;
    left:912px;
    color:#c0c0c0;
  }
  .three-screen-div {
    height:100% !important; 
    background-color:rgba(0,0,0,.4);
  }
  .hidden {
    display: none !important;
  }
  .second-onemsg{
    background: rgba(0, 0, 0, .4);
    color: #c0c0c0;
    position:relative;
    top:170px;
    height:115px;
  }
  .second-onept {
    position:relative;
    left:-304px;
  }
  .second-twpt {
    position:relative;
    left:-608px;
  }
  .second-laspt {
    position:relative;
    top:-305px;
    left:609px;
  }
  .second-lasmsg {
    position:relative;
    left:608px;
    top:-305px;
  }
  .second-as {
    position:relative;
    left:-608px;
  }
}
@media screen  and (max-width: 1269px) {
  #first-container {
    height:130px;
    overflow: hidden;
  }
  .first-small-sweet,.first-small-place,.first-small-flower,.first-small-message {
    width:20%;
    height: 130px;
    line-height: 100px;
    background-size: cover;
  }
  .onet{
    top:-230px;
    left:-7px;
    z-index:9;
  }
  .onew{
    top:-95px !important;
    right:-253px;
    z-index:9;
  }
  .onept {
    top:-236px;
    left:250px;
  }
  /* 图片丶描述容器 */
  #first-content {
  width:1060px;
  height:620px;
  padding:0 20px 0 10px;
  }
 
  /* 小模块样式 */
  #first-content .body-div{
    margin-left:4px;
    width:260px;
    height:300px;
    margin-top: 5px;
  }
 
  /* 两个描述内容小模块样式 */
  .bd-firstmsg{
    position:relative;
    background:#F4F4F4F4;
    width:240px;
    height:133px;
    margin-bottom:4px;
    z-index:999;
    text-align:left;
  }
  .bd-secondmsg{
    position:relative;
    z-index:100;
    background:#F4F4F4F4;
    width:100%;
    height:148px;
    text-align:right;
  }
  
  .first-title-left {
    left:120px;
  }
  /* 第一排最后一个描述样式 */
  .three-screen {
    float: none;
    clear: both;
    height:115px !important;
    position:relative;
    top:-135px;
    left:792px;
    color:#c0c0c0;
  }
  .three-screen-div {
    height:100% !important; 
    background-color:rgba(0,0,0,.4);
  }
  .hidden {
    display: none !important;
  }
  .second-onemsg{
    background: rgba(0, 0, 0, .4);
    color: #c0c0c0;
    position:relative;
    top:170px;
    height:115px;
  }
  .second-onept {
    position:relative;
    left:-264px;
  }
  .second-twpt {
    position:relative;
    left:-528px;
  }
  .second-laspt {
    position:relative;
    top:-305px;
    left:529px;
  }
  .second-lasmsg {
    position:relative;
    left:528px;
    top:-305px;
  }
  .second-as {
    position:relative;
    left:-528px;
  }
}

</style>
