<!DOCTYPE html>
<html>
<head>
	<script src="https://ajax.googleapis.com/ajax/libs/jquery/3.2.1/jquery.min.js"></script>
	<script>
		$(document).ready(function(){
			$("#flip").hover(function(){
				$("#panel").slideDown(0);
			});
			$("#flip").mouseleave(function(){
				$("#panel").slideUp(0);
			});
		});

	</script>
	<style>
		#panel {
			position: absolute;
			padding: 30px;
			display: none;
			background: grey;
			top: 46px;
			border-radius: 10px;
			left: 25px;
		}
		#flip {
			position: absolute;
			background: grey;
			border-radius: 10px;
			padding: 10px;
		}
		#flip:hover {
			background: #333333;
		}
	</style>
</head>
<body>

<div id="flip">Click to slide down panel</div>
<div id="panel">Hello World!</div>

</body>
</html>
