<style>
.profile {
	margin-top: 20px;
}

	img {
		max-width: 200px;
		box-shadow: 15px 15px #000;
	}

.profile-resume {
	margin-top: 20px;
}

.profile-text {
	margin-top: 15px;
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

	<div class="profile-resume">
		<h2>Resume</h2>
	</div>

	<div class="profile-text">
		<h3>Koki.O</h3>
		<h4>Location</h4>
		<p class="profile-text-description">Tokyo/Japan</p>
		<h4>Email</h4>
		<p class="profile-text-description">catjp@protonmail.ch</p>
		<h4>Jobs</h4>
		<p class="profile-text-description">Frontend Engineer</p>
		<h4>Tertiary</h4>
		<p class="profile-text-description">
			Public Management of Economics in KINDAI University<br>
			Higashiosaka City (Osaka Prefecture)<br>
			Batch 2016-2020
		</p>
		<h4>Secondary</h4>
		<p class="profile-text-description">
			Chiben Gakuen Senior High School (Nara Prefecture)<br>
			Participated in the 66th All-Japan High School Ekiden Championship<br>
			Batch 2013-2015
		</p>
	</div>

<p>The design was inspired by <a href="https://kristopolous.github.io/BOOTSTRA.386/index.html" target=”_blank”>BOOTSTRA.386</a></p>
</div>