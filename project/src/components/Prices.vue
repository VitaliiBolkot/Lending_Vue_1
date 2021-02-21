<template>
	<div class="prices">
		<h2>AND THE PRICES</h2>
		<strong>Lorem ipsum dolor sit, amet consectetur adipisicing, elit.</strong>
		<div class="main-row">
			<div class="border">
				<div class="col-prices">
					<h6>STARTER</h6>
					<strong class="strong-price">15&#8364;</strong>
					<small><strong class="strong-small">monthly</strong></small>
					<hr>
					<ul>
						<li>Text</li>
						<li>Text</li>
						<li>Text</li>
						<li>Text</li>
						<li>Text</li>
					</ul>
					<button class="btn-price">GRAB NOW</button>
				</div>
			</div>
			<div class="border">
				<div class="col-prices">
					<h6>BUSINESS</h6>
					<strong class="strong-price">30&#8364;</strong>
					<small><strong class="strong-small">monthly</strong></small>
					<hr>
					<ul>
						<li>Text</li>
						<li>Text</li>
						<li>Text</li>
						<li>Text</li>
						<li>Text</li>
					</ul>
					<button class="btn-price">GRAB NOW</button>
				</div>
			</div>
			<div class="border">
				<div class="col-prices">
					<h6>PRO</h6>
					<strong class="strong-price">50&#8364;</strong>
					<small><strong class="strong-small">monthly</strong></small>
					<hr>
					<ul>
						<li>Text</li>
						<li>Text</li>
						<li>Text</li>
						<li>Text</li>
						<li>Text</li>
					</ul>
					<button class="btn-price">GRAB NOW</button>
				</div>
			</div>
			<div class="border">
				<div class="col-prices">
					<h6>CORPORATE</h6>
					<strong class="strong-price">75&#8364;</strong>
					<small><strong class="strong-small">monthly</strong></small>
					<hr>
					<ul>
						<li>Text</li>
						<li>Text</li>
						<li>Text</li>
						<li>Text</li>
						<li>Text</li>
					</ul>
					<button class="btn-price">GRAB NOW</button>
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
.btn-price{
	margin: 2rem 0 2rem 0;
	border: none;
	color: $first-text-color;
	background-color: $color-hr-btn-border;
	padding: 7px 35px 7px 35px;
	font-family: $font-family-opensans;
	font-weight: 600;
}
li{
	font-family: $font-family-opensans;
	margin-top:5px;
	font-weight: 400;
}
hr{
	border: none;
	width: 35%;
	background-color: $color-hr-btn-border;
	height: 1px;
	margin: 1rem 0 1rem 0;
}
.strong-small{
	font-weight: 700;
}
.strong-price{
	font-size: 5rem;
	font-weight: 700;
	line-height: 75px;
}
.border{
	display:flex;
	flex-direction:column;
	justify-content:center;
	align-items:center;
	flex:1;
	padding:15px;
	border:1px solid $first-text-color;
}
h6{
	color:$color-hr-btn-border;
	font-family: $font-family-opensans;
	font-weight: 700;
	margin: 2.766667rem 0 1rem 0;
}
.main-row{
	display:flex;
	flex-direction:row;
	width:70%;
	justify-content:space-around;
	margin-top:5rem;
}
.col-prices{
	display:flex;
	flex-direction:column;
	justify-content:center;
	align-items:center;
	width:100%;
	background-color:$color-prices;
}
.col-prices:hover{
	background-color:$first-text-color;
	transition:1s;
}
.border:hover{
	background-color:$first-text-color;
	border:1px solid $color-border;
	transition:1s;
}
.prices{
	display:flex;
	flex-direction:column;
	justify-content:center;
	align-items:center;
	margin-bottom: 7rem;
}
strong{
	font-family: $font-family-opensans;
	font-weight: 600;
}
h2{
	margin-bottom:1rem;
	font-family: $font-family-bebas;
}
</style>