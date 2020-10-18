<script>
	import successkid from "../../static/inovation.png";
</script>

<style>
	figure {
		background-color: #ffffff;
	}

	h1,
	figure,
	p {
		text-align: center;
		margin: 0 auto;
	}

	h1 {
		font-size: 2.8em;
		text-transform: uppercase;
		font-weight: 700;
		margin: 0 0 0.5em 0;
	}

	figure {
		margin: 0 0 1em 0;
	}

	img {
		width: 100%;
		max-width: 400px;
		margin: 0 0 1em 0;
	}

	p {
		margin: 1em auto;
	}

	@media (min-width: 480px) {
		h1 {
			font-size: 4em;
		}
	}

	#find-button {
		background-color: #4caf50;
		border: none;
		color: white;
		padding: 15px 32px;
		text-align: center;
		text-decoration: none;
		display: inline-block;
		font-size: 16px;
	}

	#anniversaty-button {
		background-color: #cf5050;
		border: none;
		color: white;
		padding: 15px 32px;
		text-align: center;
		text-decoration: none;
		display: inline-block;
		font-size: 16px;
	}
</style>

<svelte:head>
	<title>Holistic Chamber of Commerce</title>
</svelte:head>

<h1>POOOOGGGGGG!!!!!!!!!!</h1>

<figure>
	<img alt="Success Kid" src={successkid} />
	<figcaption>This kid will find you</figcaption>
</figure>

<p><strong>Mind - Body - Spirit - Business - Budget - Planet</strong></p>

<center>
	<button id="find-button">Find holistically-minded professionals, business
		owners and resource providers!</button>
	<p />
	<button id="anniversaty-button">Our 10th Anniversary Special Event
		<strong>*IN PERSON*</strong></button>
</center>
