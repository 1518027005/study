# study
<!DOCTYPE html>
<html>
	<head>
		<meta charset="UTF-8">
		<title>jquery轮播图</title>
		<style type="text/css">
			#demo{
				width: 600px;
				height: 500px;
				border: 1px solid black;
				margin: 0 auto;
			}
			#demo2{
				width: 600px;
				height: 40px;
				border: 1px solid transparent;
				margin: 0 auto;

			}
			img{
				width: 600px;
				height: 500px;
				position: absolute;
			}
			button{
				margin: 0 50px;
				border-radius: 50%;
			}
		</style>
	</head>
	<body>
		<div id="demo">
			<img src="../day9.22/c.jpg"/>
			<img src="../day9.22/a.jpg" />
			<img src="../day9.22/4.jpg" />
			<img src="../day_921/img/4.jpg"/>
		</div>
		<div id="demo2">
			<button>1</button>
			<button>2</button>
			<button>3</button>
			<button>4</button>
		</div>
		
		
		<script src="../day9-24/js/jquery-3.4.1.js" type="text/javascript" charset="utf-8"></script>
		<script type="text/javascript">
			$(function() {
				$("button").click(function() {
					$(this).css("background-color","red").siblings().css("background-color","gray")
					var i = $(this).index()
					$("img").eq(i).fadeIn(2000).siblings().fadeOut()
					
					
					
					
					
				})
			})
		</script>
	</body>
</html>
