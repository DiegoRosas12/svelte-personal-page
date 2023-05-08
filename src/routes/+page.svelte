<script>
	import Counter from './Counter.svelte';
	import welcome from '$lib/images/svelte-welcome.webp';
	import welcome_fallback from '$lib/images/svelte-welcome.png';
</script>

<svelte:head>
	<title>Home</title>
	<meta name="description" content="Svelte demo app" />
</svelte:head>

<section>
	<nav class="bg-gray-900">
		<div class="max-w-7xl mx-auto px-4 sm:px-6 lg:px-8">
			<div class="flex items-center justify-between h-16">
				<div class="hidden md:block">
					<div class="ml-10 flex items-baseline space-x-4">
						<a
							href="/home"
							class="text-gray-300 hover:text-white px-3 py-2 rounded-md text-sm font-medium"
							>Home</a
						>
						<a
							href="/home"
							class="text-gray-300 hover:text-white px-3 py-2 rounded-md text-sm font-medium"
							>About</a
						>
						<a
							href="/home"
							class="text-gray-300 hover:text-white px-3 py-2 rounded-md text-sm font-medium"
							>Contact</a
						>
					</div>
				</div>
			</div>
		</div>
	</nav>
	<div class="max-w-7xl mx-auto py-6 sm:px-6 lg:px-8">
		<div class="px-4 py-6 sm:px-0">
			<h1 class="text-3xl font-bold text-gray-900">Diego Rosas</h1>
			<p class="mt-4 text-gray-600">
				Welcome to my portfolio! I am a skilled backend and DevOps engineer with a passion for
				creating high-quality software solutions that meet the needs of businesses and
				organizations. Welcome to my portfolio! I am a skilled backend and DevOps engineer with a
				passion for creating high-quality software solutions that meet the needs of businesses and
				organizations. My expertise lies in designing, developing, and maintaining robust and
				scalable backend systems that power web and mobile applications. I have experience with a
				wide range of technologies, including Python, Java, Node.js, and SQL databases like MySQL
				and PostgreSQL. In addition to my backend skills, I am also well-versed in DevOps practices,
				including continuous integration and deployment, automated testing, and infrastructure as
				code. I have experience with cloud computing platforms like AWS, GCP, and Azure, as well as
				with containerization technologies like Docker and Kubernetes. I believe that the key to
				success in any software project is collaboration and communication, and I pride myself on my
				ability to work closely with cross-functional teams to ensure that projects are delivered on
				time and within budget. I am a proactive problem-solver who is always looking for ways to
				improve processes and streamline workflows. If you're looking for a reliable and experienced
				backend and DevOps engineer who can help you build the infrastructure and systems you need
				to succeed, look no further. Let's work together to bring your vision to life!
			</p>
		</div>
		<div class="flex justify-center">
			<button class="bg-blue-500 hover:bg-blue-700 text-white font-bold py-2 px-4 rounded">
				Experience
			</button>
			<button class="bg-red-500 hover:bg-red-700 text-white font-bold py-2 px-4 rounded ml-4">
				Get started!
			</button>
		</div>
	</div>
	<h1>
		<span class="welcome">
			<picture>
				<source srcset={welcome} type="image/webp" />
				<img src={welcome_fallback} alt="Welcome" />
			</picture>
		</span>

		to your new<br />SvelteKit app
	</h1>

	<h2>
		try editing <strong>src/routes/+page.svelte</strong>
	</h2>

	<Counter />
</section>

<style>
	section {
		display: flex;
		flex-direction: column;
		justify-content: center;
		align-items: center;
		flex: 0.6;
	}

	h1 {
		width: 100%;
	}

	.welcome {
		display: block;
		position: relative;
		width: 100%;
		height: 0;
		padding: 0 0 calc(100% * 495 / 2048) 0;
	}

	.welcome img {
		position: absolute;
		width: 100%;
		height: 100%;
		top: 0;
		display: block;
	}
</style>
