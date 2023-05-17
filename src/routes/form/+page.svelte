
<script>
	import MAC from '$lib/assets/MAC.png';
	import HeroVideoButton from '$lib/components/hero/HeroVideoButton.svelte';
</script>

<div class='wrapper'>
	<div class="intro">
		<img class="logo" src={MAC} alt="LOGO" width="500">
		<!--     <img class="logo2" src ="MAC.png" alt="LOGO" width="500"> -->

		<div class="intro-text">
			<h1 class='title' id="title">🥾 Hiker Sign-Up 🥾</h1>
			<p
				class='description' id="description">Please fill out this form with
																						 the required
													 information for your hike.</p>
		</div>
	</div>

	<form id="survey-form" method="post" action='https://register-demo.freecodecamp.org'>



		<fieldset>

			<h1 id="personal-information">Personal Information</h1>

			<label id="name-label" for="name">Enter Your Name: <input placeholder="Enter your name" id="name" name="name"
																																type="text" required /></label>

			<label id="email-label" for="email">Enter Your Email: <input placeholder="Enter your email" id="email"
																																	 name="email" type="email" required /></label>

			<label id="number-label" for="number">Enter Your Age: <input minValue="18" maxValue="120" placeholder="Age" id="number" name="age"
																																	 type="number" required /></label>


		</fieldset>




		<fieldset>

			<h1 id="emergency-contact">Emergency Contact</h1>

			<label for="emergency-contact-name">Name:
				<input placeholder="Joe Smith" id="emergency-contact-name" name="contact-name" type="text" required /></label>


			<label for="emergency-contact-relation">Relationship:
				<input placeholder="Mother/Father..." id="emergency-contact-relation" name="contact-relation" type="text"
							 required />
			</label>

			<label for="emergency-contact-relation">Relationship:
				<input placeholder="123-456-7890" id="emergency-contact" name="phone-number" type="number" required />
			</label>

			<label for="emergency-contact-relation">Relationship:
				<input placeholder="someone@email.com" id="emergency-contact" name="phone-number" type="number"
							 required /></label>

		</fieldset>


		<h1 id="trip-details">Trip Details</h1>

		<label for="dropdown">Hiking Experience Level:
			<select id="dropdown" name="referrer">
				<option value="">(select one)</option>
				<option value="1">Beginner</option>
				<option value="2">Intermediate</option>
				<option value="3">Advanced</option>
				<option value="4">Expert</option>
			</select>
		</label>




		<fieldset> Hike Type:

			<label for="day-hike"><input id="day-hike" type="radio" name="hike-type" class="inline" /> Day Hike</label>

			<label for="multiday-hike"><input id="multiday-hike" type="radio" name="hike-type" class="inline" /> Multiday
																																																					 Trip</label>

			<label for="terms-and-conditions">
				<input id="terms-and-conditions" type="checkbox" required name="terms-and-conditions" class="inline" /> I
																																																								accept the
				<a class='text-blue-500'
					 href="https://docs.google.com/document/d/1yHrb-a4L4lOkABFHo33hNItp4fs9vbz73edBqTo--PI/edit?usp=sharing" target="_blank">terms
																																																								and conditions</a>
			</label>

		</fieldset>





		<fieldset>

			<h1 id="optional-details">Optional Details</h1>

			<label for="referrer">Number of hikes per year:
				<select id="referrer" name="referrer">
					<option value="">(select one)</option>
					<option value="1">1-5</option>
					<option value="2">5-10</option>
					<option value="3">10-15</option>
					<option value="4">15+</option>
				</select>
			</label>

			<fieldset>  What are your Favorite Trails? (Select all the apply)

				<label for="gulf-trail">
					<input value="gulf-trail" id="gulf-trail" type="checkbox" required name="trail" class="inline" /> Gulf Trail
				</label>
				<label for="cliff-trail">
					<input value="cliff-trail" id="cliff-trail" type="checkbox" required name="trail" class="inline" /> Cliff Trail
				</label>
				<label for="skylight-gully-summer">
					<input value="skylight-gully-summer" id="skylight-gully-summer" type="checkbox" required name="trail" class="inline" /> Skylight
																																																																	Gully (Summer Trail)
				</label>
				<label for="skylight-gully-winter">
					<input value="skylight-gully-winter" id="skylight-gully-winter" type="checkbox" required name="trail" class="inline" /> Skylight
																																																																	Gully (Winter Trail)
				</label>
				<label for="stary-night-trail">
					<input value="stary-night-trail" id="stary-night-trail" type="checkbox" required name="trail" class="inline" /> Stary
																																																													Night Trail
				</label>


			</fieldset>

			<label for="bio">Provide a bio:
				<textarea id="bio" name="bio" rows="3" cols="30"
									placeholder="My name is ________. I love to take trail runs..."></textarea>
			</label>

			<label for="referrer">How did you hear about us?
				<select id="referrer" name="referrer">
					<option value="">(select one)</option>
					<option value="1">MAC.org</option>
					<option value="2">Instagram</option>
					<option value="3">Facebook</option>
					<option value="4">Other</option>
				</select>
			</label>


		</fieldset>



		<input id=submit type="submit" value="Submit" />
	</form>
</div>

<div class='hero'>
	<HeroVideoButton />
</div>


<style>
		.hero{
				border-top: 3px solid #3b3b4f;
		}

    h1, p {
        margin: 1em auto;
        text-align: center;
    }

		.description{
        font-size: 1.5rem;
				width: 75%;
		}

    form {
        width: 60vw;
        max-width: 500px;
        min-width: 300px;
        margin: 0 auto;
        padding-bottom: 2em;
    }

		.title{
        text-align: center;
        font-weight: 700;
        font-size: 3rem;
		}

    fieldset {
        border: none;
        padding: 2rem 0;
        border-bottom: 3px solid #3b3b4f;
    }

    fieldset:last-of-type {
        border-bottom: none;
    }

    label {
        display: block;
        margin: 0.5rem 0;
    }


    input,
    textarea,
    select {
        margin: 10px 0 0 0;
        width: 100%;
        min-height: 2em;
        font-family: 'Mulish', sans-serif;
        border-radius: 23px 23px 23px 23px;
        -webkit-border-radius: 23px 23px 23px 23px;
        -moz-border-radius: 23px 23px 23px 23px;
        padding: 1rem;
    }

    input, textarea {
        background-color: white;
        border: 1px solid #0a0a23;
        color: black;
    }

    .inline {
        width: unset;
        margin: 0 0.5em 0 0;
        vertical-align: middle;
    }

    input[type="submit"] {
        display: block;
        width: 60%;
        margin: 1em auto;
        font-size: 16px;
        background-color: white;
        border: 7px solid #0a0a23;
        min-width: 300px;
        padding: 1.1rem;
        font-family: 'Copse', serif;
        color: black;
    }

    .logo{
        float: left;
        width: 25%;
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

    .sub-heading{
        font-size: 102px;
    }

</style>