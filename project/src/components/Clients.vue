<template>
	<div class="clients">
		<h2>CLIENTS</h2>
		<strong>Lorem, ipsum dolor, sit amet consectetur adipisicing elit.</strong>
		<div class="div-clients-logo">
			<div class="client-logo"><img src="@/assets/client-logo.png"></div>
			<div class="client-logo"><img src="@/assets/client-logo.png"></div>
			<div class="client-logo"><img src="@/assets/client-logo.png"></div>
			<div class="client-logo"><img src="@/assets/client-logo.png"></div>
			<div class="client-logo"><img src="@/assets/client-logo.png"></div>
			<div class="client-logo"><img src="@/assets/client-logo.png"></div>	
		</div>
	</div>
</template>

<script >
	export default{}
</script>

<style scoped lang="scss">
@import "@/styles/_variables.scss";
strong{
	font-family: $font-family-opensans;
	font-weight:600;
}
h2{
	margin-bottom:1rem;
	font-family: $font-family-bebas;
}
.clients{
	display:flex;
	flex-direction:column;
	align-items:center;
}
.div-clients-logo{
	display:flex;
	width:70%;
	flex-direction:row;
	justify-content:space-around;
	margin-top:5rem;
	margin-bottom:7rem;
}
</style>