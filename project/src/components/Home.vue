<template>
  <div class="row center-align ">
  	<div class="container">
    <h1>WE ARE <hr/>DESIGNING</h1>
    <h6><small>And We Are Doing It Well</small></h6>
    <button 
    class="btn-flat"
    v-on:click="scrollMeTo"
    > <i class="material-icons">expand_more</i></button>
  </div>
</div>
</template>

<script>


export default {
  methods:{
  	 scrollMeTo() {
    var element = document.getElementById("about");
    var top = element.offsetTop;

    window.scrollTo({top:top, left:0,behavior:"smooth"});
  }
  }
 
}
</script>

<style lang="scss" scoped>
@import url('https://fonts.googleapis.com/css2?family=Bebas+Neue&family=Open+Sans:wght@600&display=swap');
	hr{
		width:10rem;
	margin-top: 1rem;
    margin-bottom: 1rem;
    border: none;
    height: 3px;
    background-color: #c69b6e;
	}
	h1{
		padding-top:9rem;

		color:white;
		font-family: 'Bebas Neue', cursive;
		font-size: 7rem;
	}
	h6{
		color:white;
		font-family: 'Open Sans', sans-serif;
	}
	.material-icons{
		font-size:2rem;
	}
	button{
		border: 1px solid #ffffff;
    padding: 0px 3px 0px 3px;
    color: #c69b6e;
    margin-top: 9rem;
	}
	.row{
		margin:0;
  background-color:#2c2b2a ;
    
	}
	.container{
		padding-bottom:3rem;
	}
</style>
