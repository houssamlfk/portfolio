<script>
	let homeLink = "/";
	const changeColor = (element) => {
		let div = document.querySelector("." + element);
		div.style.transitionProperty = "background";
		div.style.transitionDuration = "0.618s";
		div.style.background = "#666666";
	};
	const changeBackColor = (element) => {
		let div = document.querySelector("." + element);
		div.style.background = "none";
	};
</script>

<body>
	<div class="header">
		<h1 class="name">Houssam Lafkih</h1>
		<div
			class="home"
			id="home"
			on:mouseover={() => {
				changeColor("home");
			}}
			on:mouseleave={() => {
				changeBackColor("home");
			}}
			on:focus
		>
			<h2><a href={homeLink}>Home</a></h2>
		</div>
		<div
			class="blog"
			on:mouseover={() => {
				changeColor("blog");
			}}
			on:mouseleave={() => {
				changeBackColor("blog");
			}}
			on:focus
		>
			<h2><a href="/blog">Blog</a></h2>
		</div>
		<div
			class="github"
			on:mouseover={() => {
				changeColor("github");
			}}
			on:mouseleave={() => {
				changeBackColor("github");
			}}
			on:focus
		>
			<h2>
				<a href="https://github.com/houssamlfk/" target="_blank"
					>Github</a
				>
			</h2>
		</div>
	</div>
	<div class="presentation">
		<div class="imgplaceholder">
			<p>This is a placeholder for an image</p>
		</div>
		<div class="about">
			<h1>I'm Houssam Lafkih, a Website Developer!</h1>
			<p>
				I am a passionate software engineer, I got into this domain by
				building simples flash games, and now I'm exploring the world of
				Web Development
			</p>
		</div>
	</div>
	<div class="techstackheader">
		<h1 class="techstacktitle">My Techstack</h1>
	</div>
	<div class="techstack">
		<div class="techitems">
			<div class="html">
				<h1>HTML</h1>
				<img
					alt="html5"
					src="vendor/html.png"
					height="128px"
					width="128px"
				/>
			</div>
			<div class="css">
				<h1>CSS</h1>
				<img
					alt="css"
					src="vendor/css.png"
					height="128px"
					width="128px"
				/>
			</div>
			<div class="express">
				<h1>expressjs</h1>
				<img
					alt="expressjs"
					src="vendor/express.png"
					height="128px"
					width="256px"
				/>
			</div>
			<div class="svelte">
				<h1>svelte</h1>
				<img
					alt="svelte"
					src="vendor/svelte.png"
					height="128px"
					width="128px"
				/>
			</div>
			<div class="sqlite">
				<h1>Sqlite</h1>
				<img
					alt="sqlite"
					src="vendor/sqlite.png"
					height="128px"
					width="128px"
				/>
			</div>
		</div>
	</div>
	<div class="projectsheader">
		<h1>Projects I've worked on</h1>
	</div>
	<div class="projects">
		<div class="firstwebsite">
			<div class="prodcorner">
				<h1>Productivity Corner</h1>
				<p>
					<a
						target="_blank"
						href="https://github.com/houssamlfk/productivity-corner"
						>My very first website</a
					> that I made, it is made using expressJs and Embedded Javascript,
					it consists of a Google OAuth session-based set of tools to ensure
					your productivity by managing your tasks and events, it is composed
					of a tasklist that communicates with a RestAPI that manages an
					SQLite database, and an online diary that is still a work in
					progress...
				</p>
			</div>
		</div>
		<div class="secondwebsite">
			<div class="portfolio">
				<h1>My Portfolio Website</h1>
				<p>
					My portfolio website that you're currently using, you can
					visit the repository<a
						target="_blank"
						href="https://github.com/houssamlfk/portfolio">here</a
					>
					!
				</p>
			</div>
		</div>
	</div>
	<div class="contactheader">
		<h1>Contact Me!</h1>
	</div>
	<div class="contact">
		<div class="email">
			<img
				alt="email"
				src="/vendor/mailicon.png"
				width="64px"
				height="64px"
			/>
			<p>Email: h.lafkih@gmail.com</p>
		</div>
		<div class="phone">
			<img
				alt="phone"
				src="/vendor/phoneicon.png"
				width="48px"
				height="48px"
			/>
			<p>Phone: +212 624 717 722</p>
		</div>
	</div>
	<footer>
		<p class="footernote">Houssam Lafkih © 2024 - Nov.</p>
	</footer>
</body>

<style>
	.header {
		position: fixed;
		display: flex;
		top: 0;
		left: 0;
		right: 0;
		align-items: center;
		padding: 0px 24px 0px 24px;
		background: linear-gradient(
			rgba(34, 34, 34, 1),
			rgba(34, 34, 34, 0.99),
			rgba(34, 34, 34, 0.98),
			rgba(34, 34, 34, 0.95),
			rgba(34, 34, 34, 0.8),
			rgba(34, 34, 34, 0.5)
		);
		margin-right: auto;
		margin-left: auto;
	}
	.home {
		padding: 8px;
	}
	.blog {
		padding: 8px;
	}
	.github {
		padding: 8px;
	}
	.name {
		margin-right: auto;
	}
	.header a {
		color: #ede7e6;
		text-decoration: none;
	}
	.presentation {
		display: flex;
		flex-direction: row;
		justify-content: center;
		background: #571000;
		gap: 12px;
		padding-top: 96px;
		padding-bottom: 12px;
		color: #ede7e6;
	}
	.presentation h1 {
		color: #ffe5b4;
	}
	.imgplaceholder {
		display: flex;
		align-items: center;
		justify-content: center;
		min-width: 300px;
		border: 2px black solid;
	}
	.about {
		display: flex;
		flex-direction: column;
		align-items: center;
		justify-content: center;
	}
	.about p {
		line-height: 35px;
		font-size: 20px;
		max-width: 400px;
	}
	.about h1 {
		font-size: 32px;
		max-width: 400px;
		text-align: center;
	}
	.projectsheader {
		display: flex;
		justify-content: center;
		background: #111111;
		color: #ede7e6;
		padding: 0;
	}
	.techstack {
		background: #571000;
	}
	.techstackheader {
		display: flex;
		justify-content: center;
		background: #111111;
		color: #ede7e6;
	}
	.projects {
		background: #571000;
		color: #ede7e6;
		display: flex;
		align-items: center;
		flex-direction: column;
	}
	.projects h1 {
		text-align: center;
		color: #ffe5b4;
	}
	.projects p {
		max-width: 900px;
		line-height: 35px;
		text-align: center;
		font-size: 20px;
	}
	.firstwebsite {
		display: flex;
		align-items: center;
	}
	.secondwebsite {
		display: flex;
		align-items: center;
	}
	.techitems {
		background: white;
		text-align: center;
		display: flex;
		justify-content: center;
	}
	.contactheader {
		display: flex;
		justify-content: center;
		background: #111111;
		color: #ede7e6;
	}
	.contact {
		display: flex;
		flex-direction: column;
		align-items: center;
		background: #571000;
		color: #ede7e6;
	}
	.phone {
		display: flex;
		align-items: center;
		gap: 8px;
	}
	.email {
		display: flex;
		align-items: center;
	}
	footer {
		display: flex;
		justify-content: center;
		background: #222222;
		color: #dddddd;
	}
	footer p {
		font-size: 13px;
	}
	h1 {
		color: #ff3e00;
		text-transform: uppercase;
		font-size: 2em;
		font-weight: 100;
	}
</style>
