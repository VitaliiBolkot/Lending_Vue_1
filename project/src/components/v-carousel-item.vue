<template>
	<div class="v-carousel-item">
		<div class="main-div">
			<div class="datas">
				<div class="div-img">
					<img v-bind:src="require('@/assets/work-img.png')">

				</div>
				<h6>CLEMENTINE DE LA FERONNIERE</h6>
				<hr>
				<small>Print Design</small>
			</div>
			<div class="datas">
			<div class="div-img">
				<img v-bind:src="require('@/assets/work-img.png')">
			</div>
			<h6>FARMER`S MARKET KITCHEN</h6>
			<hr>
			<small>Web Design</small>
			</div>
			<div class="datas">
			<div class="div-img">
				<img v-bind:src="require('@/assets/work-img.png')">
			</div>
			<h6>BEAUTIFUL GIRL</h6>
			<hr>
			<small>Photography</small>
			</div>
		</div>
	</div>
</template>

<script>

	export default{
	name:"v-carousel-item",
	props:{
		item_data:{
			type:Object,
			default:()=>{}
		}
	}
	}
</script>

<style scoped lang="scss">
@import url('https://fonts.googleapis.com/css2?family=Bebas+Neue&family=Open+Sans:wght@600&display=swap');
small{
	color:#a09f9f;
	font-family: 'Open Sans', sans-serif;
}
hr{
	display: flex;
    flex-direction: row;
    justify-content: start;
    margin-left: 0;
    width: 5rem;
    border: none;
    height: 1px;
    background-color: #c69b6e;
}
h6{
	font-family: 'Open Sans', sans-serif;
	color:#c59a6d;
	margin: 1.766667rem 0 .46rem 0;
	font-weight:600;
}
.datas{
	display:flex;
	flex-direction:column;
	margin-left:3rem;
}
.v-carousel-item{
	display:flex;
	flex-direction:column;
	justify-content:space-around;
	padding:10px;
	
}
.main-div{
	display:flex;
	flex-direction:row;
	justify-content:center;
	align-item:center;


}
.div-img{
	border:1px solid #555555;
	padding: 15px 15px 7px 15px;
	
	
}

</style>