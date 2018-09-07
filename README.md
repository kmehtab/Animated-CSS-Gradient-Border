# Animated-CSS-Gradient-Border
This is a pure css animated RGB css effect
##html code

<!DOCTYPE html>
<html>
<head>
	<title>Animation Grradient Shadow</title>
	<link rel="stylesheet" type="text/css" href="style.css">
	<link href="https://fonts.googleapis.com/css?family=Raleway:200,400" rel="stylesheet">
</head>
<body>
	<div class="shadow box">
		<p class="title">kmehtab</p>
	</div>
</body>
</html>



##css code for this


body
{
	margin: 0:
	padding: 0;
	background: #000;

}

.shadow
{	
	width:400px;
	height:250px;
	position: absolute;
	top: 0;
	bottom: 0;
	left: 0;
	right: 0;
	margin: auto;

	background: linear-gradient(0deg,#000,#262626);
}

.shadow::before,
.shadow::after
{
	content: '';
	position: absolute;
	top: -2px;
	left: -2px;
	background: linear-gradient(45deg,#fb0094,#0000ff,#00ff00,#ffff00,#ff0000,#fb0094,#0000ff,#00ff00,#ffff00,#ff0000);
	background-size: 400%;
	width: calc(100% + 4px);
	height: calc(100% + 4px);
	z-index: -1;
	animation: animate 20s linear infinite;

}
.shadow::after
{
	filter: blur(20px);
}

@keyframes animate
{
	0%
	{
		background-position: 0 0;
	}
	
	50%
	{
		background-position: 300% 0;
	}
	
	100%
	{
		background-position: 0 0;
	}
}
