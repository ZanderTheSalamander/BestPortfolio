<script>
import HeroVideoButton from '$lib/components/hero/HeroVideoButton.svelte';
import TestimonialGrid from '$lib/components/testimonial/testimonialGrid.svelte';
import TESTtestimonial from '$lib/components/testimonial/TESTtestimonial.svelte';
import HeroNumThree from '$lib/components/hero/HeroNumThree.svelte';
import PriceTable from '$lib/components/PriceTable.svelte';
import SingleTestimonial from '$lib/components/testimonial/singleTestimonial.svelte';
</script>


<HeroNumThree
	sOne='Do you want something'
	sTwo='a little different?'
/>


<div class='tribute-info' id='tribute-info'>
	<h2 class='history-title' id='history'> Who we are... </h2>
	<p class='paragraph' id='intro-summary'>
		Welcome to the Mulligan Adventure Company (MAC), your gateway to unforgettable outdoor experiences. We specialize in guided hiking trips across the US, offering a perfect blend of adventure, convenience, and comfort. With our expert guides by your side, who have extensive knowledge of the trails and local flora and fauna, you can embark on a journey where safety is ensured, and your overall experience is enhanced.

	</p>

	<div class='spacer'></div>
	<TESTtestimonial />
	<div class='spacer'></div>

	<p class='paragraph' id='intro-today'>
		MAC's meticulous planning sets us apart, as we carefully craft routes that showcase the natural wonders of each location and provide essential information prior to your trip. Whether you prefer a budget-friendly option like the "Skinny Man" plan, the comprehensive "Average Joe" plan with a guide, planned route, and prepared meals, or the all-inclusive "Muscle Man" plan covering everything including gear, we have a package tailored to meet your specific needs. Join us at the Mulligan Adventure Company and let us take care of the details while you embrace the wonders of the great outdoors. With our expert guides, meticulously planned routes, and customizable packages, we are committed to making your hiking adventure truly extraordinary.
	</p>
	<div class='spacer'></div>

</div>


<div class='spacer'></div>

<!--<TestimonialGrid />-->


<h2 class='pt-4'>But what does it cost?</h2>
<p> Take a look at our pricing below</p>

<PriceTable />

<p class='italic '>* All plans are 6 days trips in groups of 5 including the
									 guide. You
									 may
									 request specific group assignments if you are going with friends/family.
									 Travel costs to and from our outpost in New Hampshire are not included.</p>



<div class='spacer2'></div>

<SingleTestimonial />

<div class='spacer2'></div>









<div class='tribute-info' id='tribute-info'>
	<h2 class='history-title' id='history'> Our History </h2>
	<p class='paragraph' id='intro-summary'>Two families that met through their
																					kids soccer
																					team in West Hartford, Connecticut could never
																					have imaged how far they would go together. Today
																					the combined Mulligan Family (Mullins family +
																					Harrigan Family)
																					embarks	on
																					multiple Mulligan Adventure Company (MAC)
																					ski and hike trips across the US every year.</p>

	<div class='spacer'></div>

	<blockquote cite="https://www.google.com/?safe=active&ssui=on">
		<p class='quote'>"We could make some money off of this..."</p>
		<p class='by-line'>- Chris Mullins</p>
	</blockquote>

	<div class='spacer'></div>

	<p class='paragraph' id='intro-today'>Today the Mulligan Adventure Company is going strong
																				with headquarters in Marion, MA and Alpharetta, GA
																				sending hiking trips to
																				New Hampshire, Vermont and
																				California. Currently no guided ski
																				trips are offered by The Mulligan
																				Adventure Company. MAC has also recently
																				broken into the film world and is
																				starting to create short adventure
																				movies during specific trips. With so
																				much growth already and so much more
																				to come definitely keep your eye on
																				the Mulligan Adventure Company as an
																				investment and or vacation option.</p>

	<div class='spacer'></div>

</div>








<style>
    .paragraph{
        width: 85%;
        margin: auto;
        line-height: 2;
        text-align: center;
    }

    .by-line{
        text-align: center;
        font-size: 1.5rem;
        font-style: italic;
    }

    .quote{
        font-style: italic;
        font-size: 1.5rem;
        text-align: center;
    }

    .spacer {
        padding-bottom: 2rem;
    }

    .spacer2 {
        padding-bottom: 2rem;
				border-bottom: 3px solid black
    }

    .spacer3 {
        padding-bottom: 2rem;
        border-bottom: 9px solid black
    }

    h1{
        text-align: center;
        font-weight: 700;
        font-size: 3rem;
    }

    .tribute-info{
        text-align: center;
        padding-top: 1rem;
        border-bottom: 3px solid #3b3b4f;
    }

    h2 {
        font-size: 2rem;
        font-weight: 700;
        padding-bottom: 1rem;
        text-align: center;
    }
</style>