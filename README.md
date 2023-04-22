<!DOCTYPE html>
<html>
<head>
	<title>Randify</title>
	<style>
		a {
			position: absolute;
			top: calc(100vh * var(--y));
			left: calc(100vw * var(--x));
		}
	</style>
	<script>
		function randomizeLinks() {
			const links = document.querySelectorAll('a');
			for (let i = 0; i < links.length; i++) {
				links[i].style.setProperty('--x', Math.random());
				links[i].style.setProperty('--y', Math.random());
			}
		}
	</script>
</head>
<body onload="randomizeLinks()">
	<header>
		<h1>Randify</h1>
		<nav>
			<ul>
				<a href="index.html">Home</a>
				<a href="about.html">About</a>
				<a href="contact.html">Contact</a>
				<a href="blog.html">Blog</a>
			</ul>
		</nav>
	</header>
	
	<main>
		<p>lots of random stuff here</p>
	</main>
	
	<footer>
		<p>&copy; 2023 Randify.</p>
		<nav>
			<a href="https://github.com/Monardo4/randify">This page is open source, improve it!</a>
		</nav>
	</footer>
</body>
</html>
