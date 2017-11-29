<template>
	<div class="leftbar">
		<UsersList></UsersList>
			<div class="well wells">
				<img src="https://upload.wikimedia.org/wikipedia/commons/thumb/a/ae/Great_fire_of_london_map.png/500px-Great_fire_of_london_map.png" class="img-responsive">
				<h4>Clasic Address</h4>
				<p>Lorem ipsum dolor sit amet, consectetur adipisicing elit, sed do eiusmod
				tempor incididunt ut labore et dolore magna aliqua. Ut enim ad minim veniam,
				quis nostrud exercitation ullamco laboris nisi ut aliquip ex ea commodo
				</p>
				<button class="btn btn-sm btn-warning">Read More</button><br><br>
				<img src="https://static01.nyt.com/images/2017/06/23/world/23Londonfire/23Londonfire-master768.jpg" class="img-responsive">
				<h4>London Fire</h4>
				<p>Lorem ipsum dolor sit amet, consectetur adipisicing elit, sed do eiusmod
				tempor incididunt ut labore et dolore magna aliqua. Ut enim ad minim veniam,
				quis nostrud exercitation ullamco laboris nisi ut aliquip ex ea commodo
				</p>
				<button class="btn btn-sm btn-warning">Read More</button><br><br>
				<img src="https://i.ytimg.com/vi/ynncldWayqQ/maxresdefault.jpg" class="img-responsive">
				<h4>Brigadial Streng</h4>
				<p>Lorem ipsum dolor sit amet, consectetur adipisicing elit, sed do eiusmod
				tempor incididunt ut labore et dolore magna aliqua. Ut enim ad minim veniam,
				quis nostrud exercitation ullamco laboris nisi ut aliquip ex ea commodo
				</p>
				<button class="btn btn-sm btn-warning">Read More</button><br><br>
			</div>
	</div>
</template>
<script type="text/javascript">
	
	export default{
		name:'leftbar'
	}
	
</script>
<style scoped>
	.well.wells {
    background-color: transparent;
    border: transparent;
    border-radius: 1px;
    box-shadow: 0 2px 10px rgba(0,0,0,0.23);
	}
	button{
		border-radius: 50px !important;
	}
</style>