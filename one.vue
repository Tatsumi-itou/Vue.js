vue官网地址:https://cn.vuejs.org/v2/guide/syntax.html


1.如何使用vue?

	有两种方式:
		A 通过CDN或者script引入
		B 通过webpack+npm构建vue-cli脚手架	CDN地址:<script src="https://cdn.jsdelivr.net/npm/vue"></script>

2.如何实例化Vue方法?
	如果说是HTML页面的话，最外层的div都必须要有一个id，这恶id是实例化vue之后挂载的
	通过new Vue({})进行实例化
	必须要挂载到你声明div为id的和盒子上，不然不会生效

3.vue中如何初始化数据?
	在data中定义初始化变量
		注意: 在html中data是一个对象，而在单页应用开发中data是一个函数  ---->为什么呢？
		单页应用只有一个.html文件(入口文件)   之所以data是一个函数，是因为函数可以防治作用域被污染，而在多页面开发中(多尔html) 每个页面定义data为对象，页面的变量不会互相干扰	

4.Vue的生命周期函数有哪些?
	四个过程: 创建前/创建后  挂载前 /挂载后  更新前/更新后  销毁前/销毁后
	八个方法: beforCreate/created   beforeMounted/mounted  beforeUpdate/updated  beforeDestroy/destroyed

5.v-html和v-text的区别是什么?
	v-text是以字符串的形式解析		v-html是解析成html标签
