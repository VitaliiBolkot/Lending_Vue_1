<template>
	<div >
		<div class="backvideo">
<video src="@/assets/video.mp4" frameborder="0" autoplay muted loop>
	
</video>


	</div>
	<div class="sentance">
	<h4>CATHY SENTANCE</h4>
	<hr>
	<h4>WITH VIDEO BACKGROUND</h4>
	</div>
</div>
</template>

<script >
	export default{


		
	}
</script>

<style scoped lang="scss"> 
@import url('https://fonts.googleapis.com/css2?family=Bebas+Neue&family=Open+Sans:wght@400;600;700&display=swap');
hr{
	border: none;
    background-color: #c69b6e;
    width: 20%;
    height: 1px;
}
h4{
	text-align:center;
	color:white;
	font-family: 'Open Sans', sans-serif;
    font-weight: 700;
}
.sentance{
	    position: absolute;
   margin-top: -250px;
    left: 36%;
}
	.backvideo{
		width:100%;
	    opacity: 80%;
		height:350px;
		background-color:#737372;

	}
	video{
		width:100%;
		height:350px;
	}
</style>