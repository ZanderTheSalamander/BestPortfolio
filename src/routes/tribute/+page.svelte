<!-- This is a template for your tribute page -->
<script>
	import subject from '$lib/assets/MAC.png';
	import groupPhoto from '$lib/assets/groupPhoto.jpg';
	import instaPHOTO from '$lib/assets/instagram_logo_2016.svg.webp';
	import HeroImageButton from '$lib/components/hero/HeroImageButton.svelte';
</script>







<div class="intro">
	<img class="logo" src={subject} alt="LOGO" width="500">

	<div class="intro-text">
		<h1 id='title'>Mulligan Adventure Company</h1>
		<p class='sub-title' id='sub-title'>The history behind the mystery</p>
	</div>
</div>





<div class='spacer'></div>





<div class='image-container'>

<figure>
	<img class='groupPhoto' id="image" src={groupPhoto} alt="subject" />
	<figcaption class='groupPhotoCaption' id='img-caption'>MAC Members, Utah
																							2022</figcaption>
</figure>
</div>








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
										sending multiple trips per year to ski mountains in New
										Hampshire and Utah. As well as summer hiking trips to
										New Hampshire, Vermont and California. The Mulligan
																			Adventure Company has also recently
																			broken into the film world and is
																			starting to create short adventure
																			movies during specific trips. With so
																			much growth already and so much more
																			to come definitely keep your eye on
																			the Mulligan Adventure Company as an
																			investment and or vacation option.</p>

		<div class='spacer'></div>

	</div>

<div class='spacer'></div>

<div class='More-info' id='More-info'>
	<h2 class='more-info-title' id='more-info'> More Info </h2>
	<p class='paragraph' id='info-intrest'>If your interested in learning more
																				 about the Mulligan Adventure
																				 Company consider following us of
																				 Instagram, checking out our
																				 upcoming film poster, and maybe
																				 even booking a trip</p>



	<div class='flex flex-col text-center mt-10 gap-5' id='links'>

		<a class="flex place-content-center" id='instagram-link'
			 href="https://www.instagram.com"
			 target="_blank"><img class='instaLOGO hover:scale-110' id="image"
														src={instaPHOTO} alt="subject" />    </a>



		<a class="link" id='tribute-link'
			 href="https://Hut-Trip.zanderh2.repl.co"
			 target="_blank">Click here to view the poster for our upcoming film!</a>

		<HeroImageButton
			title="Are you daring enough"
			subtitle="to join us?"
			buttonText="Plans & Pricing"
		/>

		<div class='spacer'></div>

	</div>
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

		.link{
				color: darkgreen;
        text-align: center;
				font-style: italic;
		}

		.link:hover{
				color: lightgreen;
		}

	.spacer {
			padding-bottom: 2rem;
  }

    h1{
        text-align: center;
				font-weight: 700;
				font-size: 3rem;
    }

		.sub-title {
				font-size: 1.5rem;
		}

	.intro {
	display: flex;
	justify-content: space-around;
	align-items: center;
	flex-direction: row;
	border: none;
	padding: 2rem 0;
	border-bottom: 3px solid #3b3b4f;
}

	.image-container{
			display: flex;
			justify-content: center;
			align-items: center;
			flex-direction: column;
			padding: 2rem 0;

	}

  .logo{
      float: left;
      width: 25%;
  }

	.instaLOGO{
			width: 10%;

	}


	.groupPhoto{
			border: 3px solid black;
			width: max-content;
			height: max-content;
			margin: auto;
	}

	.groupPhotoCaption{
			text-align: center;
			font-style: italic;
			padding: 1rem;
      border-bottom: 3px solid #3b3b4f;
	}

	.tribute-info{
			text-align: center;
			padding-top: 1rem;
      border-bottom: 3px solid #3b3b4f;
	}

	.More-info{
			border-bottom: 3px solid #3b3b4f;
	}

	h2 {
			font-size: 2rem;
			font-weight: 700;
			padding-bottom: 1rem;
			text-align: center;
	}

</style>






