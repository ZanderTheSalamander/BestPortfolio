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
	<div class='me'>
		<slot />
		<EmailSub/>
	</div>
	<Footer/>
</div>


<style>
    .wrapper{
        background-image: url($lib/assets/mountain.jpg);
        overflow-y: auto;
        background-size: cover;
        background-position: center;
        background-attachment: fixed;
        position: fixed;
        inset: 0;
        color: black;
        font-family: 'Copse', serif;
        font-size: 16px;
        text-algin: center;
    }
    .me {
        width: 50%;
        background-color: ghostwhite;
        margin: auto auto 200px;
        padding: 20px;
        border: 10px solid black;
    }
</style>

