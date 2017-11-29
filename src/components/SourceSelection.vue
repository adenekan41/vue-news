<template>
<div class="rem">
	<div class="bgHeader">
		<div class="container-fluid">
			<h1 class="text-center t-t1"><i class="text-danger">News</i>Works<b class="t-tm">.io</b></h1>
			<h4 class="text-center t-t2">Generate Your News</h4>
		</div>
	</div>
		<div class="well wells">
			
			<div class="sourceselection">
			<h3 class="text-center">Select News Source</h3>

			<select class="form-control" v-on:change="sourceChanged">
				
				<option v-bind:value="source.id"  v-for="source in sources">{{source.name}}</option>
			</select>
		</div>
		<div v-if="source">
			<h5>{{source.description}}</h5>
			<a v-bind:href="source.url" class="btn btn-warning" style="border-radius: 50px;s" target="_blank">Go to Website</a><br><br>
		</div>
	</div>
	</div>
</template>

<script type="text/javascript">
	
	export default{
		name: 'sourceselection',

		data (){
			return{
			sources: [],
			source: ''
			}
			
		},
		methods: {
			sourceChanged: function(e){
				for (var i =0; i <this.sources.length; i++) {
					if (this.sources[i].id === e.target.value) {
						this.source = this.sources[i];	
					}

				}
				this.$emit('sourceChanged', e.target.value)
			}
		},
		created: function () {
			// body...
			this.$http.get('https://newsapi.org/v1/sources?language=en')
			.then(response => {
				this.sources = response.data.sources;
			})
		}
	}
</script>

<style scoped>
	.bgHeader{
		background-image:linear-gradient(rgba(0,0,0,0.63),rgba(0,0,0,0.63)),url(https://images.pexels.com/photos/209137/pexels-photo-209137.jpeg?w=940&h=650&auto=compress&cs=tinysrgb) ;
		width: 100%;
		height: 150px;
		min-width: 100%;
		max-width: 100%;
		background-size: cover;
		background-attachment: fixed;
	}
	.t-t1{
		color: white;
		font-size: 3.2em;
		padding-top: 5%;
		text-transform: uppercase;
		font-weight: 400;
		-webkit-font-smoothing:antialised;
		font-smooth: always;
		
	}
	.t-t2{
		color: white;

	}
	.t-tm{
		color: white;
		font-size: ;
		font-weight: 100;

	}
	.well.wells {
    background-color: transparent;
    border: transparent;
    border-radius: 1px;
    box-shadow: 0 2px 10px rgba(0,0,0,0.23);
	}
</style>