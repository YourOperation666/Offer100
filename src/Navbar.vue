<template>
<nav align="right" id="Navbar">
	<span v-for="item in navList"><a v-bind:href="''+item.url">{{item.label}}</a></span>
</nav>
</template>

<style type="text/css" scoped>
nav{
	width: 100%;
	background-color: #333;
	height: 1.8em;
	line-height: 1.8em;
	color:white;
}
nav > span{
	color:#aaa;
	font-size: 10pt;
	padding-right: 0.5em;
	padding-left: 0.5em;
	border-right: 1px solid #aaa;
}
nav > span:last-child{
	border: none;
}
a{
	color: #aaa;
	text-decoration: none;
}
</style>
<script type="text/javascript">
export default{
	name:'Navbar',
	data(){
		return{
			navList:[
				{label:"Messgae",url:"#"},
				{label:"My PR",url:"#"},
				{label:"Delivery Box",url:"#"},
				{label:"Collection",url:"#"},
				{label:"User",url:"#"}]
		}
	}
}
</script>