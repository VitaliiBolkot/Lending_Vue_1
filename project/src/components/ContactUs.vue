<template>
	<div class="contact-us">
		<h2>CONTACT US</h2>
		<strong>Lorem, ipsum dolor, sit amet consectetur adipisicing elit.</strong>
		<div class="main-row">
			<form class="col s12" @submit.prevent="sendRequest">
				<div class="row">
					<div class="input-field col s4">
						<input placeholder="Your Name" v-model="name" type="text" class="validate">
					</div>
					<div class="input-field col s4">
						<input v-model="email" placeholder="Your Email" type="email" class="validate">
						<span class="helper-text" data-error="wrong" data-success="right"></span>
					</div>
					<div class="input-field col s4">
						<input v-model="phone" type="number" class="validate" placeholder="Your Phone">
					</div>
				</div>
				<div class="row">
					<div class="input-field col s12">
						<textarea v-model="textarea" class="materialize-textarea"></textarea>
						<label for="textarea1">Textarea</label>
					</div>
				</div>
				<div class="btn-div">
					<input class="btn-input" type="submit" value="SEND THE MESSAGE">
				</div>
			</form>
		</div>
	</div>
</template>

<script>
	export default{
		data(){
			return {
				name: '',
				email: '',
				phone: '',
				textarea:'',
			}
		},
		methods:{
			sendRequest(){	
			}
		}
	}
</script>

<style scoped lang="scss">
@import "@/styles/_variables.scss";
.btn-input{
	padding:20px 20px 20px 20px;
	padding: 10px 40px 10px 40px;
	color: $first-text-color;
	background-color: $color-hr-btn-border;
	border: none;
	font-weight: 600;
	font-family: $font-family-opensans;
	outline:none;
}
.btn-div{
	display:flex;
	flex-direction:row;
	justify-content:center;
	margin-bottom: 7rem;
}
.contact-us{
	display:flex;
	flex-direction:column;
	align-items:center;
}
h2{
	margin-bottom:1rem;
	margin-top:5rem;
	font-family: $font-family-bebas;
}
strong{
	font-family: $font-family-opensans;
	font-weight:600;

}
.main-row{
	display:flex;
	flex-direction:column;
	align-items:center;
	margin-top: 5rem;
}
</style>