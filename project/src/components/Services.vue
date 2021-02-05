<template>
	<div class="services">
		<h2>SERVICES</h2>
		<strong>Lorem ipsum dolor sit, amet consectetur adipisicing, elit.</strong>
		<div class="main-row">
			<div class="service-col">
				<div class="div-icon">
					<div><img src="@/assets/services-1-icon.png" alt=""></div>
				</div>
				<h6>DESIGN & ART DIRECTING</h6>
				<small>Lorem ipsum dolor sit amet consectetur adipisicing elit. Iure quidem voluptates iste dolores dolorum? Deleniti explicabo perspiciatis, quam neque possimus quo quaerat. Accusamus rerum error atque et impedit, velit tempora.</small>
			</div>
			<div class="service-col">
				<div class="div-icon">
					<div><img src="@/assets/services-2-icon.png" alt=""></div>
				</div>
				<h6>DEVELOPING</h6>
				<small>Lorem ipsum dolor sit amet consectetur, adipisicing elit. Dignissimos deserunt neque, ea quisquam qui illo reiciendis harum beatae optio voluptas voluptate atque quo ducimus architecto in distinctio officiis tempora impedit?</small>
			</div>
			<div class="service-col">
				<div class="div-icon">
					<div><img src="@/assets/services-3-icon.png" alt=""></div>
				</div>
				<h6>CONSULTING</h6>
				<small>Lorem ipsum dolor sit amet consectetur, adipisicing elit. Deleniti amet quam mollitia quasi quo, possimus quas autem distinctio modi impedit consectetur quidem incidunt, neque expedita reiciendis accusantium non suscipit qui.</small>
			</div>
		</div>
		<hr>
	</div>
</template>


<script>
	export default{

	}
</script>


<style scoped lang="scss">
@import url('https://fonts.googleapis.com/css2?family=Bebas+Neue&family=Open+Sans:wght@600&display=swap');

	hr{
		    width: 10%;
    border: none;
    height: 1px;
    background-color: #cccccc;
    margin-top: 5rem;
    margin-bottom: 5rem;
	}
	.div-icon{
		border:1px solid #cccccc;
		width:130px;
		height:130px;
		display:flex;
		flex-direction:row;
		justify-content:center;
		align-items:center;
	}
	h6{
		color:#d4b392;
		font-family: 'Open Sans', sans-serif;
	}
	small{
		font-family: 'Open Sans', sans-serif;
		text-align:center;
		padding-left: 3rem;
    	padding-right: 3rem;
    	padding-top:2rem;
	}
	strong{
		font-family: 'Open Sans', sans-serif;
	}
	h2{
		margin-bottom:1rem;
		margin-top:4rem;
		font-family: 'Bebas Neue', cursive;
	}
	.main-row{
		margin-top:5rem;
		display:flex;
		flex-direction:row;
		justify-content:space-between;
		width:70%;
		align-items:center
	}
	.services{
		display:flex;
		flex-direction:column;
		justify-content:center;
		align-items:center;
	}
	.service-col{
		display:flex;
		flex-direction:column;
		justify-content:center;
		flex:1;
		align-items:center;
		
	}
</style>