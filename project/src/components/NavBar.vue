<template>
	<nav>
    <div class="nav row">
    	<div class="col s3 ">
      <img  src="@/assets/logo.png" alt=""></div>
      <div class="col s9">
      <ul class="right">
        <li>
        	<a href="#">
        		<strong>
        			<span class="active_span">HOME</span>
        		</strong>
        	</a>
        </li>
        <li><a href="#about"><strong>ABOUT</strong></a></li>
        <li><a href="#services"><strong>SERVICES</strong></a></li>
        <li><a href="#works"><strong>WORKS</strong></a></li>
        <li><a href="#prices"><strong>PRICING</strong></a></li>
        <li><a href="#clients"><strong>CLIENTS</strong></a></li>
        <li><a href="#blog"><strong>BLOG</strong></a></li>
        <li><a href="#contact"><strong>CONTACT</strong></a></li>
      </ul></div>
    </div>
  </nav>
</template>

<script>
	export default{

	}
</script>

<style lang="scss" scoped>
	li{
		font-style:bold;
		
	}
	img{
		width:75px;
	}
	.nav{
		padding-left:10rem;
		padding-right:10rem;
		justify-content:center;
		background-color:#2c2b2a;
		}
	
	.active_span{
		border:1px solid #ffffff;
		color:#bc9262;
		padding: 0.5rem 1rem 0.5rem 1rem;
	}
	.row{
		background-color:#2c2b2a;
		
		margin:0;
 
	}
	nav{
		box-shadow:0px 0px;
	}
	
</style>