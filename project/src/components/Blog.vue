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
	export default{}
</script>

<style scoped lang="scss">
@import "@/styles/_variables.scss";
span{
	font-family: $font-family-opensans;
	font-size: 55px;
	color: $first-text-color;
	font-weight: 700;
	line-height: 1;
}
strong{
	font-family: $font-family-opensans;
	font-weight:600;
	color:$first-text-color;
}
h6{
	margin: 0;
	color:$color-h6;
	font-weight:700;
	font-family: $font-family-opensans;
}
h2{
	margin-bottom:1rem;
	color:$first-text-color;
	font-family: $font-family-bebas;
}
.blog{
	display:flex;
	flex-direction:column;
	align-items:center;
	background-color:$bg-color;
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