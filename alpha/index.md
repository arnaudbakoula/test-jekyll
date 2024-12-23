---
layout: "alpha"
title: "Alpha"
permalink: "alpha/"
header_class: "alt"
---


<!-- Main -->
<section id="main" class="container ">
	<section class="box special">
		<header class="major">
			<h2>Introducing the ultimate mobile app
			<br />
			for doing stuff with your phone</h2>
			<p>Blandit varius ut praesent nascetur eu penatibus nisi risus faucibus nunc ornare<br />
			adipiscing nunc adipiscing. Condimentum turpis massa.</p>
		</header>
		<span class="image featured"><img src="images/pic01.jpg" alt="" /></span>
	</section>
	<section class="box special features">
		<div class="features-row">
			<section>
				<span class="icon solid major fa-bolt accent2"></span>
				<h3>Magna etiam</h3>
				<p>Integer volutpat ante et accumsan commophasellus sed aliquam feugiat lorem aliquet ut enim rutrum phasellus iaculis accumsan dolore magna aliquam veroeros.</p>
			</section>
			<section>
				<span class="icon solid major fa-chart-area accent3"></span>
				<h3>Ipsum dolor</h3>
				<p>Integer volutpat ante et accumsan commophasellus sed aliquam feugiat lorem aliquet ut enim rutrum phasellus iaculis accumsan dolore magna aliquam veroeros.</p>
			</section>
		</div>
		<div class="features-row">
			<section>
				<span class="icon solid major fa-cloud accent4"></span>
				<h3>Sed feugiat</h3>
				<p>Integer volutpat ante et accumsan commophasellus sed aliquam feugiat lorem aliquet ut enim rutrum phasellus iaculis accumsan dolore magna aliquam veroeros.</p>
			</section>
			<section>
				<span class="icon solid major fa-lock accent5"></span>
				<h3>Enim phasellus</h3>
				<p>Integer volutpat ante et accumsan commophasellus sed aliquam feugiat lorem aliquet ut enim rutrum phasellus iaculis accumsan dolore magna aliquam veroeros.</p>
			</section>
		</div>
	</section>
	<div class="row">
		<div class="col-6 col-12-narrower">
			<section class="box special">
				<span class="image featured"><img src="images/pic02.jpg" alt="" /></span>
				<h3>Sed lorem adipiscing</h3>
				<p>Integer volutpat ante et accumsan commophasellus sed aliquam feugiat lorem aliquet ut enim rutrum phasellus iaculis accumsan dolore magna aliquam veroeros.</p>
				<ul class="actions special">
					<li><a href="#" class="button alt">Learn More</a></li>
				</ul>
			</section>
		</div>
		<div class="col-6 col-12-narrower">
			<section class="box special">
				<span class="image featured"><img src="images/pic03.jpg" alt="" /></span>
				<h3>Accumsan integer</h3>
				<p>Integer volutpat ante et accumsan commophasellus sed aliquam feugiat lorem aliquet ut enim rutrum phasellus iaculis accumsan dolore magna aliquam veroeros.</p>
				<ul class="actions special">
					<li><a href="#" class="button alt">Learn More</a></li>
				</ul>
			</section>
		</div>
	</div>
	<section class="box special features">
		<div class="features-row">
			<h2>Section avec 4 encarts</h2>
		</div>
		<div class="features-row">
		{% for service in site.data.alpha.services %}
			<section>
				<h3>{{ service.offer }}</h3>
				<p>{{ service.description }}</p>
				<ul style="list-style-position: inside; text-align:left; margin-left:5%; margin-right:5%">
					{% for option in service.options %}
					<li>{{ option.duration }} minutes at {{ option.price }}</li>
					{% endfor %}
				</ul>
				<hr/>
				<ul class="actions special">
					<li><a href="#" class="button alt">Book</a></li>
				</ul>
			</section>
		{% endfor%}
		</div>
	</section>
	<section class="box special">
		<div class="row">
		{% for service in site.data.alpha.services %}
			<div class="col-4 col-12-mobilep">
				<h3>{{ service.offer }}</h3>
				<p>{{ service.description }}</p>
				<div style="text-align:left">
				<ul>
					{% for option in service.options %}
					<li style="list-style-position: inside; text-align:left; margin-left:5%; margin-right:5%">{{ option.duration }} minutes at {{ option.price }}</li>
					{% endfor %}
				</ul>
				</div>
				<hr/>
				<ul class="actions special">
					<li><a href="#" class="button alt">Book</a></li>
				</ul>
			</div>
		{% endfor%}
		</div>
	</section>
</section>
<section class="cta">
	<h2>Our Services</h2>
	<p>Blandit varius ut praesent nascetur eu penatibus nisi risus faucibus nunc.</p>
</section>
<section class="container">
	<div class="row">
	{% for service in site.data.alpha.services %}
		<div class="col-4 col-12-narrower">
			<section class="box special">
				<span class="image featured"><img src="images/pic04.jpg" alt="" /></span>
				<h3>{{ service.offer }}</h3>
				<p>{{ service.description }}</p>
				<ul style="list-style-position: inside; text-align:left; margin-left:5%; margin-right:5%">
					{% for option in service.options %}
					<li>{{ option.duration }} minutes at {{ option.price }}</li>
					{% endfor %}
				</ul>
				<hr/>
				<ul class="actions special">
					<li><a href="#" class="button alt">Book</a></li>
				</ul>
				</section>
			</div>
	{% endfor%}
	</div>
	<div class="row">
		<div class="col-12">
		<section class="box special">
		<p>Something here</p>
			{% for person in site.data.alpha.persons %}
				<span><a href="#">{{ person.name }}</a></span>
			{% endfor %}
		</section>
		</div>
	</div>
</section>

<!-- CTA -->
<section id="cta">
	<h2>Sign up for beta access</h2>
	<p>Blandit varius ut praesent nascetur eu penatibus nisi risus faucibus nunc.</p>
	<form>
		<div class="row gtr-50 gtr-uniform">
			<div class="col-8 col-12-mobilep">
				<input type="email" name="email" id="email" placeholder="Email Address" />
			</div>
			<div class="col-4 col-12-mobilep">
				<input type="submit" value="Sign Up" class="fit" />
			</div>
		</div>
	</form>
</section>