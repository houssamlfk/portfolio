<script>
	let homeLink = "/";
	const changeColorAndText = (element) => {
		let div = document.querySelector("." + element);
		let text = document.querySelector("." + element + " h2");
		div.style.transitionProperty = "background";
		text.style.transitionProperty = "font-size";
		text.style.fontSize = "28px";
		text.style.transitionDuration = "0.3s";
		div.style.transitionDuration = "0.618s";
		div.style.background = "purple";
	};
	const changeBackColorAndText = (element) => {
		let div = document.querySelector("." + element);
		let text = document.querySelector("." + element + " h2");
		text.style.fontSize = "24px";
		div.style.background = "none";
	};
	const changeBackColor = (element) => {
		let div = document.querySelector("." + element);
		div.style.background = "#160022";
	};
	const changeColor = (element) => {
		let div = document.querySelector("." + element);
		div.style.transitionProperty = "background";
		div.style.transitionDuration = "0.618s";
		div.style.background = "#320040";
	};
</script>

<body>
	<div class="firstscreen">
		<div class="header">
			<h1 class="name">Houssam Lafkih</h1>
			<div
				class="home"
				id="home"
				on:mouseover={() => {
					changeColorAndText("home");
				}}
				on:mouseleave={() => {
					changeBackColorAndText("home");
				}}
				on:focus
			>
				<h2><a href={homeLink}>Home</a></h2>
			</div>
			<div
				class="blog"
				on:mouseover={() => {
					changeColorAndText("blog");
				}}
				on:mouseleave={() => {
					changeBackColorAndText("blog");
				}}
				on:focus
			>
				<h2><a href="/blog">Blog</a></h2>
			</div>
			<div
				class="github"
				on:mouseover={() => {
					changeColorAndText("github");
				}}
				on:mouseleave={() => {
					changeBackColorAndText("github");
				}}
				on:focus
			>
				<h2>
					<a href="https://github.com/houssamlfk/" target="_blank"
						>Github</a
					>
				</h2>
			</div>
			<div class="resume">
				<button class="resumebtn">Resume</button>
			</div>
		</div>
		<div class="presentation">
			<div class="presentationitems">
				<div class="about">
					<h1>
						Designing responsive websites that suit your taste and
						needs.
					</h1>
				</div>
			</div>
		</div>
	</div>
	<div
		class="techstack"
		on:mouseover={() => {
			changeColor("techstack");
		}}
		on:focus
		on:mouseleave={() => {
			changeBackColor("techstack");
		}}
	>
		<div class="techstackheader">
			<h1 class="techstacktitle">My Techstack</h1>
			<div class="techstacktrait">00000000000</div>
		</div>
		<div class="techitems">
			<div class="row1">
				<div class="html">
					<img
						alt="html5"
						src="vendor/html.svg"
						height="128px"
						width="128px"
					/>
					<h1>HTML</h1>
				</div>
				<div class="css">
					<img
						alt="css"
						src="vendor/css.svg"
						height="128px"
						width="128px"
					/>
					<h1>CSS</h1>
				</div>
				<div class="javascript">
					<img
						alt="javascript"
						src="vendor/js.svg"
						height="128px"
						width="128px"
					/>
					<h1>Javascript</h1>
				</div>
			</div>
			<div class="row2">
				<div class="express">
					<img
						alt="expressjs"
						src="vendor/express.svg"
						height="128px"
						width="128px"
					/>
					<h1>expressjs</h1>
				</div>

				<div class="svelte">
					<img
						alt="svelte"
						src="vendor/svelte.svg"
						height="128px"
						width="128px"
					/>
					<h1>svelte</h1>
				</div>
				<div class="sqlite">
					<img
						alt="sqlite"
						src="vendor/sqlite.png"
						height="128px"
						width="128px"
					/>
					<h1>Sqlite</h1>
				</div>
			</div>
		</div>
	</div>

	<div
		class="projects"
		on:mouseover={() => {
			changeColor("projects");
		}}
		on:focus
		on:mouseleave={() => {
			changeBackColor("projects");
		}}
	>
		<div class="projectsheader">
			<h1>Projects I've worked on</h1>
			<div>00000000</div>
		</div>
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
						href="https://github.com/houssamlfk/portfolio"
					>
						here</a
					>
					!
				</p>
			</div>
		</div>
	</div>
	<div
		class="contact"
		on:mouseover={() => {
			changeColor("contact");
		}}
		on:mouseleave={() => {
			changeBackColor("contact");
		}}
		on:focus
	>
		<div class="contactheader">
			<h1>Contact Me!</h1>
			<div>000000000</div>
		</div>
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
		display: flex;
		align-items: center;
		padding: 0px 24px 0px 24px;
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
	.header h1 {
		padding-top: 6px;
		font-weight: 500;
		color: #d690fc;
		font-family:
			system-ui,
			-apple-system,
			BlinkMacSystemFont,
			"Segoe UI",
			Roboto,
			Oxygen,
			Ubuntu,
			Cantarell,
			"Open Sans",
			"Helvetica Neue",
			sans-serif;
	}
	.header a {
		color: #eedcfe;
		text-decoration: none;
	}
	.resume {
		padding-top: 8px;
		margin-left: 50px;
	}
	.resumebtn {
		background-color: cyan;
		border-radius: 40px;
		color: #160020;
		border: transparent;
	}
	.firstscreen {
		background-size: 1920px 1080px;
		min-height: 100%;
		background-image: url("/vendor/parallax.jpg");
	}
	.presentation {
		display: flex;
		flex-direction: row;
		justify-content: center;
		gap: 12px;
		padding-top: 190px;
		padding-bottom: 12px;
		color: #ede7e6;
	}
	.presentationitems {
		display: flex;
		align-items: center;
	}
	.presentation h1 {
		color: #ffe5b4;
	}
	.row1 {
		display: flex;
		justify-content: center;
		align-items: center;
		gap: 72px;
	}
	.row2 {
		display: flex;
		justify-content: center;
		align-items: center;
		gap: 72px;
	}
	.about {
		background: rgba(0, 0, 0, 0);
		display: flex;
		flex-direction: column;
		align-items: center;
		justify-content: center;
		border-radius: 12px;
	}
	.about h1 {
		text-transform: none;
		font-weight: 400;
		background-image: linear-gradient(to left, #94fbff, #ff7df0);
		color: transparent;
		background-clip: text;
		font-size: 55px;
		max-width: 800px;
	}
	.projectsheader {
		display: flex;
		justify-content: center;
		flex-direction: column;
		padding-bottom: 24px;
	}
	.projectsheader h1 {
		font-size: 40px;
		color: transparent;
		background-image: linear-gradient(to left, #94fbff, #ff7df0);
		background-clip: text;
	}
	.projectsheader div {
		color: transparent;
		background-image: linear-gradient(to left, #94fbff, #ff7df0);
		font-size: 8px;
		line-height: 8px;
	}
	.techstack {
		background: #160020;
		display: flex;
		align-items: center;
		flex-direction: column;
	}
	.techstackheader {
		display: flex;
		justify-content: center;
		flex-direction: column;
		padding-bottom: 24px;
	}
	.techstackheader div {
		color: transparent;
		background: linear-gradient(to left, #94fbff, #ff7df0);
		border-radius: 40px;
		font-size: 8px;
		line-height: 8px;
	}
	.techstackheader h1 {
		font-size: 40px;
		color: transparent;
		background-image: linear-gradient(to left, #94fbff, #ff7df0);
		background-clip: text;
	}
	.projects {
		background: #160020;
		display: flex;
		align-items: center;
		flex-direction: column;
	}
	.firstwebsite,
	.secondwebsite h1 {
		text-align: center;
		color: #94fbff;
	}
	.projects p {
		max-width: 900px;
		line-height: 35px;
		text-align: center;
		font-size: 20px;
		color: #eeccee;
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
		text-align: center;
		display: flex;
		flex-direction: column;
		justify-content: center;
		padding-top: 24px;
	}
	.techitems h1 {
		text-transform: none;
		color: pink;
	}
	.contactheader {
		display: flex;
		justify-content: center;
		flex-direction: column;
		padding-bottom: 24px;
	}
	.contactheader div {
		color: transparent;
		background-image: linear-gradient(to left, #94fbff, #ff7df0);
		border-radius: 40px;
		font-size: 8px;
		line-height: 8px;
	}
	.contactheader h1 {
		color: transparent;
		background-image: linear-gradient(to left, #94fbff, #ff7df0);
		background-clip: text;
		font-size: 40px;
	}
	.contact {
		display: flex;
		flex-direction: column;
		align-items: center;
		background: #160020;
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
		background: #000000;
		color: #dddddd;
	}
	footer p {
		font-size: 13px;
	}
	body {
		margin: 0;
		padding: 0;
		background: white;
	}
</style>
