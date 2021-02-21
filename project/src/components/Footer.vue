<template>
	<div class="footer">
		<div class="footer-data"><small>Copyright © 2014 Trendy - Designed by Stefan Parnarov</small></div>
		<div class="icons">
			<img src="@/assets/footer-icon-1.png" alt="">
			<img src="@/assets/footer-icon-2.png" alt="">
			<img src="@/assets/footer-icon-3.png" alt="">
			<img src="@/assets/footer-icon-4.png" alt="">
			<img src="@/assets/footer-icon-5.png" alt="">
			<img src="@/assets/footer-icon-6.png" alt="">
			<img src="@/assets/footer-icon-7.png" alt="">
			<img src="@/assets/footer-icon-8.png" alt="">
			<img src="@/assets/footer-icon-9.png" alt="">
		</div>
	</div>
</template>

<script >
	export default{

	}
</script>

<style scoped lang="scss">
@import "@/styles/_variables.scss";
	.footer{
		display:flex;
		flex-direction:row;
		justify-content:space-around;
		padding:20px;
	}
	.footer-data{
font-family: $font-family-opensans;
    display: flex;
    flex-direction: column;
    align-items: center;
    justify-content: center;
	}
	img{
		padding: 10px;
	}
	.icons{
		display: flex;
    align-items: center;
	}
</style>