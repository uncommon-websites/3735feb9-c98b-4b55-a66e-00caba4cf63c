<script lang="ts">
	// Components
	import CallToAction from "$lib/components/layout/CallToAction.svelte";

	// Icons
	import StakeholderGrid from "$lib/components/layout/StakeholderGrid.svelte";
	import Story from "./Story.svelte";
	import SecondaryHero from "$lib/components/layout/hero-sections/SecondaryHero.svelte";
	import Culture from "$lib/components/layout/Culture.svelte";

	// Constants
	const values = [
		{
			title: "Innovation",
			description: "Constantly challenging the status quo to create better solutions."
		},
		{
			title: "Integrity",
			description: "Building trust through transparent actions and honest communication."
		},
		{
			title: "Impact",
			description: "Measuring our success by the positive change we create for our clients."
		}
	];
</script>

<SecondaryHero
	title="Your open source AI employee"
	subtitle="Automate research, sales, hiring, and more with a generalist agent that works across the web"
	imageSrc="/mockups/airport-screen-1749639985552.png"
/>

<!-- Story Section -->
<Story
	paragraphs={[
		"We created Suna because we kept running into the same problem—too much time spent on repetitive, online work. From digging through websites for research to manually gathering data, it was clear there had to be a better way to offload this kind of busywork and focus on higher-value thinking. Sound familiar?",
		"Suna is our answer. It's a generalist AI agent that works on your behalf—finding leads, drafting emails, planning trips, extracting data, and more. It handles a broad scope of digital tasks fully autonomously, like having a smart, tireless assistant who learns quickly and never misses a step. Suna helps individuals and teams do more, with fewer distractions.",
		"We're building Suna in the open. It's 100% open source, licensed under Apache 2.0, and available on GitHub. Anyone can use it, host it, improve it, or contribute to it. We're a growing, global community of builders, tinkerers, and professionals making everyday work a little less manual—for everyone."
	]}
/>

<!-- Our Culture Section -->
<Culture {values} />

<!-- StakeholderGrid Section -->
<StakeholderGrid
	stakeholderType="team"
	title="Our community."
	subtitle="Built by contributors from around the world."
	stakeholders={[]}
>
	<div class="text-center max-w-xl mx-auto mt-8">
		<h3 class="text-lg font-semibold mb-2">A global open source project</h3>
		<p class="mb-4 text-body">Suna by Kortix is built and improved every day by a diverse group of open-source contributors. There is no classic org chart—just a growing, global collective making AI autonomy accessible to everyone. Anyone can join, contribute, or suggest ideas. All progress happens in the open on <a href="https://github.com/kortix-ai/suna" target="_blank" class="underline">GitHub</a>.</p>
		<p class="font-medium">Interested in shaping the future of autonomous AI? <a href="https://github.com/kortix-ai/suna" target="_blank" class="underline">Contribute or get involved</a>.</p>
	</div>
</StakeholderGrid>


<StakeholderGrid
	stakeholderType="investor"
	title="Proudly independent."
	subtitle="Community-owned. No outside investors."
	stakeholders={[]}
>
	<div class="text-center max-w-xl mx-auto mt-8">
		<h3 class="text-lg font-semibold mb-2">No investors. No hidden agenda.</h3>
		<p class="mb-4 text-body">Suna by Kortix is entirely community-owned, open source, and independent. There are no external investors or corporate backers. Every line of code and every decision happens in the open—with full transparency, for the benefit of everyone.</p>
		<p><a href="https://github.com/kortix-ai/suna" target="_blank" class="underline">See our progress on GitHub</a></p>
	</div>
</StakeholderGrid>


<!-- CTA Section -->
<CallToAction
	title="Ready to collaborate?"
	subtitle="Let's create something amazing"
	description="Join the companies already leveraging our expertise to transform their digital presence and achieve their business goals."
/>
