<template>
<div>
	<nav-header :active="active"></nav-header>
	<!-- 并非采用后台动态添加，后期增加动态修改 -->
	<el-row type="flex" justify="center" class="about_content">
		<el-col :span="15" class="about">
			<el-card class="box-card">
				<h1>About Blog</h1>
				<hr class="line"/>
    			<p>简单介绍下博客使用技术：</p>
    			<p class="about_title">博客前端：</p>
    			<p class="about_text"><b>采用服务器端渲染(ssr)</b>,基于 Vue.js 的通用应用框架:<b>Nuxt.js + Element-UI + @nuxtjs/axios + Less</b></p>
    			<p class="about_title">博客后端:</p>
    			<p class="about_text">UI层：使用 <b>Vue + Vue-Router + Vue-cli + Vue + Axios + Less + Iview</b></p>
    			<p class="about_text">服务层：使用 <b>Node.js + Koa2 + MongoDB + Mongoose + Koa-session</b></p>
    			<h1>About Me</h1>
				<hr class="line"/>
				<p class="about_title">个人简介</p>
				<ul>
					<li>姓名：qianchaochushui</li>
				</ul>
				<p class="about_title">技能</p>
				<ul>
					<li>前端：HTML、CSS、Javacript(ES next)、JQuery、Vue全家桶、微信小程序开发、Hybrid APP混合开发等等</li>
					<li>UI框架：Bootstrap、Vux、Element-UI,Iview 等等</li>
					<li>后端：NodeJs、MongoDB+Mongoose、mysql+sequlize,Express、Koa2</li>
				</ul>
				<p class="about_title">个人评价</p>
				<p class="about_text">好好学习，天天向上</p>
			</el-card>
		</el-col>
	</el-row>
</div>
</template>

<script>
import NavHeader from '@/components/NavHeader.vue'
export default {
	data() {
		return {
			active:'about'
		}
	},
	components:{
		NavHeader
	},
  head() {
    return {
      title:'qianchaochushui的个人博客-一个基于Nuxt构建的博客网站',
      meta:[
        {hid:'description',
          name:'description',
          content:'qianchaochushui个人博客，是一个记录博主学习和成长的自媒体博客。关注于web前端技术和web全栈技术的学习研究。'},
        {hid:'keywords',name:'keywords',
          content:'qianchaochushui,互联网,自媒体,博客,新鲜科技,科技博客,独立博客,个人博客,原创博客,前端,前端开发,全栈,全栈开发,koa,nuxt,nuxtjs,vue,vuejs'},
        {hid:'author',content:'qianchaochushui'}
      ]
    }
  }
}
</script>

<style lang="less" scoped>
	@import './../../assets/css/Index/About.less';
</style>
