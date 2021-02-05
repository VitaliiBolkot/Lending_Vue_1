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
					<p>+359 2 88 55 999 <br/> +359 89  88 55 999</p>
				</div>
			</div>
			<div class="data-div">
				<div class="div-img">
					<img src="@/assets/office-address.png" alt="">
				</div>
				<div class="data-img">
					<h6>OFFICE ADDRESS</h6>
					<p>4 Byala Cherkva Str. <br>
3rd Floor <br>
Sofia, 1000,  <br>
Bulgaria</p>
				</div>					
			</div>
			<div class="data-div">
				<div class="div-img">
					<img src="@/assets/email.png" alt="">
				</div>
				<div class="data-img">
					<h6>EMAILS</h6>
					<p>office@trendy.com <br>
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
@import url('https://fonts.googleapis.com/css2?family=Bebas+Neue&family=Open+Sans:wght@600&display=swap');
	h2{
		margin-bottom:1rem;
		margin-top:5rem;
		font-family: 'Bebas Neue', cursive;
		color:white;
	}
	strong{
		font-family: 'Open Sans', sans-serif;
		font-weight:600;
		color:white;
		
	}
	.find-us{
		display:flex;
		flex-direction:column;
		align-items:center;
		background-color:#2c2b2a;
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
    color: #bb9369;
    font-weight: 700;
    font-family: 'Open Sans', sans-serif;
	}
	p{
		color:white;
		 font-family: 'Open Sans', sans-serif;
	}
</style>