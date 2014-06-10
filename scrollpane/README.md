# Hero Carousel

Installation
===

### Step 1: Build the HTML

This is the basic structure of Carousel:

	<div class="hero">
			<div class="hero-carousel">
				<article>
					<img src="slide-1.jpg" alt="slide 1" width="980" height="550" />
					<div class="contents">
						<h1>Hero Carousel...</h1>
						<p>Sed pharetra, nulla ac blandit hendrerit, justo lacus tempus leo, non fermentum elit tellus at enim.</p>
					</div>
				</article>
				<article>
					<img src="slide-2.jpg" alt="slide 2" width="980" height="550" />
					<div class="contents">
						<h1>...a jQuery carousel plugin...</h1>
						<p>Quisque cursus consequat risus vel sollicitudin. Nam ut mauris at dui bibendum pretium facilisis nec enim.</p>
					</div>
				</article>
				<article>
					<img src="slide-3.jpg" alt="slide 3" width="980" height="550" />
					<div class="contents">
						<h1>...with 100% width &amp; <br />previews of next/previous slide!</h1>
						<p>Proin ultricies, ipsum at congue dapibus, justo augue egestas tortor, sit amet varius velit massa at nunc.</p>
					</div>
				</article>
			</div>
		</div>
		
### Step 2: Link the Required Files

By default, Hero Carousel requires jQuery Easing (1.3+). Other than that, it only requires the CSS file and `jquery.heroCarousel-1.3.js` javascript file.

	<!-- Hero Carousel CSS -->
	<link rel="stylesheet" media="all" href="jquery.heroCarousel.css" type="text/css" />
	
	<!-- Hero Carousel JS -->
	<script src="jquery.easing-1.3.js"></script>
	<script src="jquery.heroCarousel-1.3.js"></script>
	
### Step 3: Initialize Hero Carousel

Put this (preferably) at the bottom of your `body` tag:

	<script>
			$(document).ready(function(){
				$('.hero-carousel').heroCarousel({
					easing: 'easeOutExpo',
					css3pieFix: true
				});
			});
	</script>