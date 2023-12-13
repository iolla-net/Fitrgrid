# .FITRGRID

![fitrgrid logo](https://github.com/wachilt/Fitrgrid/blob/master/images/icons/retina.png)


## A small screen first flexbox CSS grid

Fitrgrid is a fork of fitgrd, a lightweight responsive grid by Jan Müller, and inherits all features of the original.  

Fitrgrid is divided into twelve percentage-based columns. Each column has a two percent gutter. Fitrgrid comes with a single media query (for viewports wider than 640px) that you can adjust or supplement to taste.

#### → [FITRGRID PREVIEW](http://wachilt.github.io/Fitrgrid)

##  How does Fitrgrid differ from fitgrd?  
I've worked with the original fitgrd and love it's simplicity. However, I now take a mobile-first approach to web development and wanted fitgrd to match these principles. I dismantled and reconfigured fitgrd as the new mobile-first Fitrgrid.

Fitrgrid has been (re)built from the ground up for small screen first web development and adds a new extra-wide grid option. Fitrgrid CSS weighs in at the same 4KB (uncompressed) file size of the original project and works well with modern mobile and desktop web browsers - some older ones too.

## NEW: Flexbox retrofit. Floats and clearfix begone!


##  Basic Setup 
To add Fitrgrid to your website, simply include `fitrgrid.pack.css` into your document's `<head>`

To guarantee a perfect responsive grid, follow these specs:

- container (`header`, `div`, `article`, `footer` etc.)
	- class center
		- class row
			- classes fg1 - fg12 as required
			
			
##  Markup example
````html
<header>
	<div class="center">
		<div class="row">
			<section class="fg2">
				your logo
			</section>
			<section class="fg10">
				page navigation would go here
			</section>
		</div>
	</div>
</header>

<article class="your-class-name">
	<div class="center">
		<div class="row">
			<section class="fg4"> lorem ipsum ... </section>
			<section class="fg4"> lorem ipsum ... </section>
			<section class="fg4"> lorem ipsum ... </section>		
		</div>
	</div>
</article>

<footer>
	<div class="center">
		<div class="row">
			<section class="fg6"> footer copyright </section>
			<section class="fg6"> footer navigation </section>
		</div>
	</div>
</footer>

````

##  Utility classes
For the moment Fitrgrid keeps it simple with just 4 utility classes:

| Utility class      | Description
| -----------|---
| .fg-no-gutter | Perfect for big edgeless image grids
| .fg-no-mobile | Do not display content on small screen devices
| .fg-no-desktop | Do not display content on large screen devices
| .fg-wide _(new!)_ | Full-width edgeless grids constrained by .center class width (default 1280px)

Fitrgrid will feature additional utility classes in future.

##  Compatibility  
Fitrgrid works well in all modern web browsers.

##  Acknowledgement 
Thank you to Jan Müller for the original fitgrd project.
