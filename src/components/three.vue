<template>
  <div id="three">
		<header>
			<div class="header_menu">
				<ul>
					<li>
						<img src="/static/images/ftc.png"/>
					</li>
					<li><router-link to= "/">首页</router-link></li>
					<li><router-link to= "/four">盒子我们</router-link></li>
					<li><router-link to= "/five">留言板</router-link></li>
					<li><router-link to= "/second">概率事件</router-link></li>
				</ul>
			</div>
      <div></div>
		</header>
    <div id="form">
      <el-form :model="chickenMsg" :inline="true">
        <el-form-item>
          <el-upload
            class="avatar-uploader"
            ref="uploadImage"
            action="https://jsonplaceholder.typicode.com/posts/"
            :show-file-list="false"
            :on-change="changeImage"
            :on-success="uploadSuccess" 
            :auto-upload="false"
            name="image">
            <img v-if="imageUrl" :src="imageUrl" class="avatar">
            <i v-else class="el-icon-plus avatar-uploader-icon"></i>
          </el-upload>
        </el-form-item>
        <el-form-item>
          <el-input
            style="width:98%;"
            type="textarea"
            :autosize="{ minRows: 13, maxRows: 13}"
            placeholder="请输入内容"
            v-model="chickenMsg.msg">
          </el-input>
        </el-form-item>
        <el-form-item>
          <el-button type="success" @click="submitMsg">成功按钮</el-button>
        </el-form-item>
      </el-form>  
    </div>
  </div>    
</template>
<script>
export default {
	name: 'four',
	data() {
		return {
      imageUrl: '',
      chickenMsg: {
        image: '',
        msg: '',
        time: ''
      }
		}
  },
  methods: {
    changeImage(file, fileList) {
      this.imageUrl = URL.createObjectURL(file.raw);
      console.log('this.imageUrl:' + this.imageUrl)
    },
    uploadSuccess() {
      this.$refs.uploadImgs.clearFiles()
    },
    submitUpload() {
      this.$refs.uploadImage.submit()
    },
    submitMsg() {
      console.log('this.chickenMsg.msg:'+this.chickenMsg.msg)
    }
  }
}
</script>
<style>
@charset "UTF-8";
#three header {
	overflow-x: hidden;
  position: relative;
  width: 100%;
  height: 100%;
	margin: 0 auto;
  background: rgb(179, 177, 192);
}
a {
	text-decoration: none;
	color: #18314F;
}
#three ul {
	margin: 0;
	padding: 0;
}
#three li {
	list-style: none;
	margin: 0;
	padding: 0;
}
#three header ul li {
	width: 20%;
	float: left;
	line-height: 60px;
}
#three header ul li:first-child {
	text-align: left;
}
#three header ul li img {
	height:60px;
}
#three header div {
	width: 100%;
	height:60px;
}
#three header .header_menu {
	position: fixed;
	z-index: 9;
  background: rgb(249, 249, 253);
}
.el-form {
  width: 600px;
  margin: 20px auto;
}
.avatar-uploader .el-upload {
    width: 320px;
    height: 280px;
    border: 1px dashed #d9d9d9;
    border-radius: 6px;
    cursor: pointer;
    position: relative;
    overflow: hidden;
}
.avatar-uploader .el-upload:hover {
  border-color: #409EFF;
}
.avatar-uploader-icon {
  font-size: 28px;
  color: #8c939d;
  width: 290px;
  height: 260px;
  line-height: 260px;
  text-align: center;
}
.avatar {
  width: 100%;
  height: 100%;
  display: block;
  object-fit: cover;
}
@media only screen and (min-width: 300px) and (max-width: 460px) {
  .avatar-uploader .el-upload {
    width: 96%;
    height: 420px;
  }
  .el-form {
    width: 96%;
    margin:auto;
  }
  .el-form-item,.el-form-item__content {
    width:100%;
  }
  #three #form {
    margin: 20px 0 0 0;
  }
  #three header ul li {
		font-size: 14px;
	}
}
</style>


