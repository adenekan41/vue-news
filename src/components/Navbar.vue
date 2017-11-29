<template>
	<div class="navbar">
		<header>
			<nav class="navbar navbar-inverse navbar-static-top">
			  <div class="container-fluid">
			    <div class="navbar-header">
			      <button type="button" class="navbar-toggle" data-toggle="collapse" data-target="#myNavbar">
			        <span class="icon-bar"></span>
			        <span class="icon-bar"></span>
			        <span class="icon-bar"></span>                        
			      </button>
			      <a class="navbar-brand" href="#" style="color: white;"><i class="text-danger">News</i>Works</a>
			    </div>
			    <div class="collapse navbar-collapse" id="myNavbar">
			      <ul class="nav navbar-nav">
			        <li class="active"><a href="#">Home</a></li>
			        <li class="dropdown">
			          <a class="dropdown-toggle" data-toggle="dropdown" href="#">News <span class="caret"></span></a>
			          <ul class="dropdown-menu">
			            <li><a href="#">Top 1-1</a></li>
			            <li><a href="#">Latest 1-2</a></li>
			            <li><a href="#">Porpular 1-3</a></li>
			          </ul>
			        </li>
			        <li><a href="#">Api Key</a></li>
			        <li><a href="#">FAQ</a></li>
			      </ul>
			      <ul class="nav navbar-nav navbar-right">
			        <li><a href="#"><span class="glyphicon glyphicon-user"></span> Sign Up</a></li>
			        <li><a href="#"><span class="glyphicon glyphicon-log-in"></span> Login</a></li>
			      </ul>
			    </div>
			  </div>
			</nav>
  
		</header>
	</div>
</template>
<script type="text/javascript">
	export default{
		name: 'navbar'
	}
</script>
<style scoped>
	.navbar {
    position: relative;
    min-height: 50px;
    background-color: transparent;
    /* margin-bottom: 20px; */
    /* border: 1px solid transparent; */
}
.navbar-inverse {
    background-color: transparent;
    border-color: transparent !important;
}
.navbar-inverse>li>a {
    color: white;
}
.navbar-inverse .navbar-nav>li>a {
    color: #fff;
}
</style>