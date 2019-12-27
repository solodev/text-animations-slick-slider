# text-animations-slick-slider
Adding text animations to your slider can help emphasize content and create smooth transitions between slides.

## Tutorial
For detailed instruction's, view Solodev's [Using Text Animations with Slick Slider](https://www.solodev.com/blog/web-design/using-text-animations-with-slick-slider.stml) article.

## Demo
Try out a working example on [JSFiddle](https://jsfiddle.net/solodev/b1fg3y8d/).

## HTML
The tutorial contains the following basic HTML markup.
```
   <header class="hero-text">
	<div class="hero" data-arrows="true" data-autoplay="true">
	  <!--.hero-slide-->
	
	  <div class="hero-slide">
         <img alt="Mars Image" class="img-responsive cover" src="https://raw.githubusercontent.com/solodev/text-animations-slick-slider/master/images/rocket.jpg">
         <div class="header-content text-white position-absolute slide-content col-lg-4">
            <h1 class="mb-4">Be part of the <span class="d-block font-weight-bold">Lunar XPerience</span></h1>  
            <a class="btn btn-primary btn-lg w-max mt-2" href="#" tabindex="0">Tour Our Ships</a>
         </div>
	  </div>
	  <!--.hero-slide-->
	
	  <div class="hero-slide">
          <img alt="Mars Image" class="img-responsive cover" src="https://raw.githubusercontent.com/solodev/text-animations-slick-slider/master/images/mars-mission.jpg">
          <div class="header-content text-white position-absolute slide-content col-lg-4">
                <h1 class="mb-4">LunarXP Voted Best Mars Mission</h1>  
                <p class="font-weight-bold">Inc. magazine today ranked LunarXP as the fastest growing company in the Mars Mission category.</p>
                <a class="btn btn-primary btn-lg w-max mt-2" href="#" tabindex="0">Read More</a>
             </div>
	  </div>
	  <!--.hero-slide-->
	
	  <div class="hero-slide">
          <img alt="Mars Image" class="img-responsive cover" src="https://raw.githubusercontent.com/solodev/text-animations-slick-slider/master/images/cosmos.jpg">
          <div class="header-content text-white position-absolute slide-content col-lg-4">
                <p>Our fleet of advanced spacecraft have revolutionized the lunar economy and provided safe travel for thousands of scientists, engineers, technicians, medical staff and civilians. These amazing vessels are also paving the way for reaching Mars in the next decade.</p>  
				<a class="btn btn-primary btn-lg w-max mt-2" href="#" tabindex="0">Read More</a>
			</div>
	  </div>
	</div><!--.hero-->
  </header>	
```
## Javascript
```
	jQuery(document).ready(function ($) {
	  $('.hero').slick({
		dots: true,
        infinite: true,
        speed: 500,
        fade: !0,
        cssEase: 'linear',
		slidesToShow: 1,
		slidesToScroll: 1,
        autoplay: true,
		autoplaySpeed: 8000,
        draggable: false,
		arrows: false,
		responsive: [
	    {
		breakpoint: 1024,
		settings: {
		slidesToShow: 1,
		slidesToScroll: 1,
        infinite: true
		          }
        },
        {
		breakpoint: 768,
		settings: {
        draggable: true,
		          }
		},
		{
		breakpoint: 600,
		settings: {
        slidesToShow: 1,
        draggable: true,
		slidesToScroll: 1
			      }
		},
		{
		breakpoint: 480,
		settings: {
        slidesToShow: 1,
        draggable: true,
		slidesToScroll: 1
		          }
		}
	
			      ]
                  });
        });		
```

## CSS
All required CSS is contained with style.css

## External Resources
This tutorial includes the following third party resources.

```
<link rel="stylesheet" href="https://stackpath.bootstrapcdn.com/bootstrap/4.1.3/css/bootstrap.min.css" integrity="sha384-MCw98/SFnGE8fJT3GXwEOngsV7Zt27NXFoaoApmYm81iuXoPkFOJwJ8ERdknLPMO" crossorigin="anonymous">
<link rel="stylesheet" type="text/css" href="https://cdn.jsdelivr.net/npm/slick-carousel@1.8.1/slick/slick.css" />
<script src="https://code.jquery.com/jquery-3.3.1.slim.min.js" integrity="sha384-q8i/X+965DzO0rT7abK41JStQIAqVgRVzpbzo5smXKp4YfRvH+8abtTE1Pi6jizo" crossorigin="anonymous"></script>
<script src="https://stackpath.bootstrapcdn.com/bootstrap/4.1.3/js/bootstrap.min.js" integrity="sha384-ChfqqxuZUCnJSK3+MXmPNIyE6ZbWh2IMqE241rYiqJxyMiZ6OW/JmZQ5stwEULTy" crossorigin="anonymous"></script>
<script type="text/javascript" src="https://cdn.jsdelivr.net/npm/slick-carousel@1.8.1/slick/slick.min.js"></script>
```