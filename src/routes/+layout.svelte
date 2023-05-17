<!--This is a wrapper around all other content on your website. Things here
should be on every page, such as a header, footer, or the loading of global
styles.-->
<!--Also required by Tailwind CSS to load in the global Tailwind Styles.-->
<script>
  import "../app.css";
	import Header from '$lib/components/Header.svelte';
	import Footer from '$lib/components/Footer.svelte';
	import EmailSub from '$lib/components/emailSub.svelte';
</script>


<!--This is the main content on every page-->

<div class='wrapper'>
	<Header/>
	<div class="container">
		<div class="MainPage">
			<div class='me'>
				<slot />
			</div>
		</div>
		<div class="Sidebar">
			<EmailSub/>
		</div>
	</div>
	<Footer/>
</div>

<style>
    .wrapper{
        background-image: url($lib/assets/mountain.jpg);
        overflow-y: auto;
				overflow-x: hidden;
        background-size: cover;
        background-position: center;
        background-attachment: fixed;
        position: fixed;
        inset: 0;
        color: black;
        font-family: 'Copse', serif;
        font-size: 16px;
        text-align: center;
				display: flex;
				flex-direction: column;
				align-items: center;
    }
    .me {
        width: 100%;
        background-color: ghostwhite;
        margin: auto auto 200px;
        padding: 20px;
        border: 10px solid black;
    }

    .container {
				min-width: 100%;
				display: grid;
				margin: 10px;
        grid-template-columns: 25% 50% 25%;
        grid-template-rows: 25% 25% 25% 25%;
        gap: 0px 0px;
        grid-auto-flow: row;
        grid-template-areas:
    "Sidebar MainPage ."
    ". MainPage ."
    ". MainPage ."
    ". MainPage .";
				padding: 0 20px;
    }

    .MainPage { grid-area: MainPage; }

    .Sidebar { grid-area: Sidebar; }


</style>

