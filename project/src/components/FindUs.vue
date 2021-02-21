<template>
	<div class="find-us">
		<h2>FIND US</h2>
		<strong>Lorem, ipsum dolor, sit amet consectetur adipisicing elit.</strong>
		<div class="main-row">
			<div class="data-div">
				<div class="div-img">
					<img src="@/assets/phone.png" alt="">
				</div>
				<div class="data-img">
					<h6>PHONES</h6>
					<p>+359 2 88 55 999</p>  <p>+359 89  88 55 999</p>
				</div>
			</div>
			<div class="data-div">
				<div class="div-img">
					<img src="@/assets/office-address.png" alt="">
				</div>
				<div class="data-img">
					<h6>OFFICE ADDRESS</h6>
					<p>4 Byala Cherkva Str. 
					3rd Floor </p>
					<p>
					Sofia, 1000,  
					Bulgaria</p>
				</div>					
			</div>
			<div class="data-div">
				<div class="div-img">
					<img src="@/assets/email.png" alt="">
				</div>
				<div class="data-img">
					<h6>EMAILS</h6>
					<p>office@trendy.com</p> <p>
					sales@trendy.com</p>
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
@import "@/styles/_variables.scss";
h2{
	margin-bottom:1rem;
	margin-top:5rem;
	font-family: $font-family-bebas;
	color: $first-text-color;
}
strong{
	font-family: $font-family-opensans;
	font-weight:600;
	color: $first-text-color;

}
.find-us{
	display:flex;
	flex-direction:column;
	align-items:center;
	background-color:$bg-color;
}
.main-row{
	display:flex;
	flex-direction:row;
	justify-content:space-around;
	width:70%;
	margin-top: 5rem;
	margin-bottom: 7rem;
}
.data-div{
	display:flex;
	flex-direction:row;
	justify-content:center;
	align-items: start;
}
.data-img{
	padding-left:40px;
	padding-right:40px;
}
h6{
	margin: 0;
	color: $color-h6;
	font-weight: 700;
	font-family: $font-family-opensans;
}
p{
	color: $first-text-color;
	font-family: $font-family-opensans;
}
</style>