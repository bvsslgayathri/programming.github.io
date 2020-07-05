# programming.github.io
welcome to programming
<!DOCTYPE html>
<html>
<head>
<style type="text/css">
	*
{

margin: 0;
padding: 0;

}
.web
{
height: 100vh;
width: 100%;
background: url(sky.jpg);
background-size:cover;
background-position: center;
position: relative;
overflow-x: hidden;

}
.highway
{
	height: 200px;
	width: 500%;
	display: block;
	background-image: url(road.jpg);
	position: absolute;
	bottom: 0;
	left: 0;
	right: 0;
	z-index: 1;
	background-repeat: repeat-x;

	animation: highway 10s linear infinite;

}
.city
{
	height: 200px;
	width: 500%;
	display: block;
	background-image: url(city.jpg);
	position: absolute;
	bottom: 0;
	left: 0;
	right: 0;
	z-index: 1;
	background-repeat: repeat-x;
	animation: city 20s linear infinite;

}
.car{
	width: 400px;
	left: 50%;
	bottom: 99px;
	transform: translate(-50%);
	position: absolute;
	z-index: 2;
}
.car img
{
	width: 100%;
	animation: car 1s linear infinite;
}
.wheel
{
	left: 50%;
	bottom:178px;
	transform: translateX(-50%);
	position: absolute;
	z-index: 2;

}
.wheel img
{
	width: 72px;
	height: 72px;
	animation: wheel 1s linear infinite;
}
.back-wheel{
	left:-165px;
	position: absolute;
}
.front-wheel{
	left:80px;
	position: absolute;
}
@keyframes wheel
{
	100%{
		transform: rotate(360deg);
			}
}
@keyframes car{
100%{
	transform: translateY(-1px);
}
50%{
	transform: translateY(1px);
}
0%{
	transform: translateY(-1px);
}
}
@keyframes city
{
	100%{
		transform: translateX(-3400px);
	}
}

@keyframes highway
{
	100%{
		transform: translateX(-3400px);
	}
}


</style>
	<link rel="stylesheet" type="text/css" href="web.css">
	<title></title>
</head>
<body>
<div class="web">
	<div class="highway">
		
	</div>
	<div class="city"></div>
	<dir class="car">
		<img src="car.png">
	</dir>
	<div class="wheel">
		<img src="wheel.png" class="back-wheel">
		<img src="wheel.png" class="front-wheel">
	</div>
</div>
</body>
</html>
