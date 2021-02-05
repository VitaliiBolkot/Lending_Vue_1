<template>
	<div class="blog">
		<h2>SOME COOL FACTS</h2>
		<strong>Lorem, ipsum dolor, sit amet consectetur adipisicing elit.</strong>
		<div class="div-facts">
			<div class="div-fact">
				
				<div class="div-fact-img">
					<img src="@/assets/happy-clients.png" alt="">
				</div>
		
				<div class="div-fact-data">
					<span>120</span>
					<h6>HAPPY CLIENTS</h6>
				</div>
				
			</div>
			<div class="div-fact">
				<div class="div-fact-img">
					<img src="@/assets/awesome-projects.png" alt="">
				</div>
				<div class="div-fact-data">
					<span>551</span>
					<h6>AWESOME PROJECTS</h6>
				</div>
				
			</div>
			<div class="div-fact">
				<div class="div-fact-img">
					<img src="@/assets/working-hours.png" alt="">
				</div>
				<div class="div-fact-data">
					<span>95K</span>
					<h6>WORKING HOURS</h6>
				</div>
				
				</div>
			<div class="div-fact">
				<div class="div-fact-img">
					<img src="@/assets/coffes-drinked.png" alt="">
				</div>
				<div class="div-fact-data">
					<span>1.2K</span>
					<h6>COFFES DRINKED</h6>
				</div>
				
		</div>
		</div>
	</div>
</template>

<script>
	export default{

	}
</script>

<style scoped lang="scss">
@import url('https://fonts.googleapis.com/css2?family=Bebas+Neue&family=Open+Sans:wght@600&display=swap');
	span{
	font-family: 'Open Sans', sans-serif;
    font-size: 55px;
    color: white;
    font-weight: 700;
   line-height: 1;
	}
	strong{
		font-family: 'Open Sans', sans-serif;
		font-weight:600;
		color:white;
	}
	h6{
		margin: 0;
		color:#bb9369;
		font-weight:700;
    font-family: 'Open Sans', sans-serif;
	}
	h2{
		margin-bottom:1rem;
		color:white;
		font-family: 'Bebas Neue', cursive;
	}
	.blog{
		display:flex;
		flex-direction:column;
		align-items:center;
		background-color:#2c2b2a;
	}
	.div-facts{
		display:flex;
		flex-direction:row;
		justify-content:space-around;
		width:70%;
		margin-top: 5rem;
		margin-bottom: 5rem;
	}
	.div-fact{
		display:flex;
		flex-direction:row;
		justify-content:center;
		align-items: baseline;
	}
	.div-fact-data{
		    padding-left: 25px;
    padding-right: 25px;
	}
</style>