<template>
	<div class="row center-align ">
		<div class="container">
			<h1>WE ARE <hr/>DESIGNING</h1>
			<h6><small>And We Are Doing It Well</small></h6>
			<button class="btn-flat" @:click="scrollMeTo"> <i class="material-icons">expand_more</i></button>
	</div>
</div>
</template>

<script>
	export default {
		methods:{
			scrollMeTo() {
				var element = document.getElementById("about");
				var top = element.offsetTop;
				window.scrollTo({top:top, left:0,behavior:"smooth"});
			}
		}
	}
</script>

<style lang="scss" scoped>
@import "@/styles/_variables.scss";
hr{
	width:10rem;
	margin-top: 1rem;
	margin-bottom: 1rem;
	border: none;
	height: 3px;
	background-color: $color-hr-btn-border;
}
h1{
	padding-top:9rem;
	color:$first-text-color;
	font-family: $font-family-bebas;
	font-size: 7rem;
}
h6{
	color:$first-text-color;
	font-family: $font-family-opensans;
}
.material-icons{
	font-size:2rem;
}
button{
	border: 1px solid $first-text-color;
	padding: 0px 3px 0px 3px;
	color: $color-hr-btn-border;
	margin-top: 9rem;
}
.row{
	margin:0;
	background-color:$bg-color;
}
.container{
	padding-bottom:3rem;
}
</style>
