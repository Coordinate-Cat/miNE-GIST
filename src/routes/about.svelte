<style>
.profile {
	margin-top: 20px;
}

	img {
		max-width: 200px;
		box-shadow: 15px 15px #000;
	}

.profile-text {
	margin-top: 20px;
}

.profile-text-description {
	color: #55FF55
}
</style>

<svelte:head>
	<title>About</title>
</svelte:head>

<h1>About me</h1>

<div class="profile">
	<img src="me.png" alt="me">

	<h2>Resume</h2>

	<div class="profile-text">
		<h3>Location</h3>
		<p class="profile-text-description">Tokyo/Japan</p>
		<h3>Email</h3>
		<p class="profile-text-description">catjp@protonmail.ch</p>
		<h3>Jobs</h3>
		<p class="profile-text-description">Frontend Engineer</p>
	</div>

<p>The design was inspired by <a href="https://kristopolous.github.io/BOOTSTRA.386/index.html" target=”_blank”>BOOTSTRA.386</a></p>
</div>