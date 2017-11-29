<template>
	
	<div class="newslist">
		<div class="">
			<ul class="media-list"> 
				<li class="media" v-for="article in articles">
					<div class="media-left">
						<a v-bind:href="article.url" target="_blank"><img v-bind:src="article.urlToImage" class="media-object"></a>
						<h5><i>by {{article.author}}</i></h5>
					</div>
					
					<div class="media-body">
						<div class="well wells">
							<h4 class="media-heading">
								<a v-bind:href="article.url
								" target="_blank">{{article.title}}</a>
							</h4>
							<h5><i>by {{article.author}}</i></h5>
							<p>{{article.description}} <a v-bind:href="article.url" target="_blank">Read More</a></p>
							<p>{{article.publishedAt}}</p>
						</div>
					</div>
				</li>
			</ul>
		</div>
	</div>
</template>

<script type="text/javascript">
	
	export default{
		name: 'newslist',
		props:['source'],
		data (){
			return{
				articles:[]
			}
		},
		methods:{
			updateSource: function (source) {
				this.$http.get('https://newsapi.org/v1/articles?source=' + source + '&apiKey=bea44bd884944f598946adf913577392')
				.then(response =>{
					this.articles = response.data.articles;
				});
			}
		},
		created: function(){
			this.updateSource(this.source);
		},
		watch:{
			source: function(val){
				this.updateSource(val);
			}
		}
	}
</script>


<style scoped>
	.media-object{
		width: 18em;
		padding: 10px;

	}
	.media{
		border-top: 1px solid grey;
		padding-top: 20px;
	}
	.well.wells {
    background-color: transparent;
    border: transparent;
    border-radius: 1px;
    box-shadow: 0 2px 10px rgba(0,0,0,0.23);
	}
	.media {
    border-top: 1px solid #eee;
    padding-top: 20px;
}
</style>
