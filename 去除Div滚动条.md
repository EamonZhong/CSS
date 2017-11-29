今天在工作中遇到一个坑，就是div的滚动条特别的low，对于解决这个办法，我们可以使用插件，但是今天无意之中发现了一个比较简单的方法，如果你不需要div的滚动条但是却有滚动效果的话就要看看下面这个方法了。     

	<div class="box">
		<ul class="inner-box">
			<li class="list-item">。。。。</li>
		</ul>
	</div>     
	<style>
		.box
			width: 100px
			height: 200px
			overflow hidden
			.inner-box
				height: 100%
			  	width: 120px
			  	overflow-y: auto
			  	overflow-x: hidden
				.list-item
					height: 40px
					width: 100px
					overflow: hidden 
	</style>

这样的话滚动条就会消失而且依旧有滚动效果。当然要不要这个滚动条还是根据需求来定。