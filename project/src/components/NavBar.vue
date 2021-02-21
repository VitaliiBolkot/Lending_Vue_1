<template>
<nav>
	<div class="nav row">
		<div class="col ">
			<img  src="@/assets/logo.png" alt="">
		</div>
		<div class="col">
			<ul class="right">
				<li><a @click="scrollMeTo('#')"><strong><span class="active_span">HOME</span></strong></a></li>
				<li><a @click="scrollMeTo('about')"><strong><span class="active_span">ABOUT</span></strong></a></li>
				<li><a @click="scrollMeTo('services')"><strong><span class="active_span">SERVICES</span></strong></a></li>
				<li><a @click="scrollMeTo('works')" ><strong><span class="active_span">WORKS</span></strong></a></li>
				<li><a @click="scrollMeTo('prices')" ><strong><span class="active_span">PRICING</span></strong></a></li>
				<li><a @click="scrollMeTo('clients')" ><strong><span class="active_span">CLIENTS</span></strong></a></li>
				<li><a @click="scrollMeTo('blog')" ><strong><span class="active_span">BLOG</span></strong></a></li>
				<li><a @click="scrollMeTo('contact')"><strong><span class="active_span">CONTACT</span></strong></a></li>
			</ul>
		</div>
		</div>
	</nav>
</template>

<script>
	export default{
		methods:{
			scrollMeTo(id) {
				var element = document.getElementById(id);
				var top = element.offsetTop;
				window.scrollTo({top:top, left:0,behavior:"smooth"});
			}
		}
	}
</script>

<style lang="scss" scoped>
@import "@/styles/_variables.scss";
li{
	font-style:bold;
}
ul{
	
	display: flex;
	width: 100%;
	flex-direction: row;
	justify-content: space-betwee
}
img{	width:75px;		}
.nav{
	padding-left:10rem;
	padding-right:10rem;
	justify-content:center;
	background-color:$bg-color;
}
.active_span{
	padding: 0.5rem;
	border:1px solid #bg-color;

}
.active_span:hover{
	border:1px solid $first-text-color;
	color:$color-nav-text;
	transition:0.5s;
}
.row{
	display: flex;
	flex-direction: row;
	justify-content: space-between;
	margin:0;
}
nav{
	box-shadow:0px 0px;
	background-color:$bg-color;
}
</style>