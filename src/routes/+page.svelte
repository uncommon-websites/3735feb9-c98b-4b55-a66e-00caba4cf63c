<script lang="ts">
	// Components
	import UseCases from "$lib/components/layout/UseCases.svelte";
	import Summary from "$lib/components/layout/Summary.svelte";
	import Features from "$lib/components/layout/Features.svelte";
	import Testimonials from "$lib/components/layout/Testimonials.svelte";
	import CallToAction from "$lib/components/layout/CallToAction.svelte";
	import AboutTeaser from "$lib/components/layout/AboutTeaser.svelte";
	import LogoScroller from "$lib/components/layout/LogoScroller.svelte";
	import CustomerCardHero from "$lib/components/layout/hero-sections/CustomerCardHero.svelte";
</script>

<CustomerCardHero
  centered={true}
  title="More time, fewer tabs"
  subtitle="Suna completes time-consuming tasks like lead generation, market research, recruitment, and trip planning—so you can focus on real work, not repetitive clicks."
  customers={[
    {
      name: "Maria Herrera, sales manager at Fyricom",
      position: undefined,
      imageSrc: "/generated/image-a-professional-latina-sales-manager-in-a.webp",
      testimonial: "Suna saves us 10+ hours a week on lead research. What used to be a risky, error-prone manual process is now done in minutes."
    },
    {
      name: "Duke Park, people ops lead at Vessa Labs",
      position: undefined,
      imageSrc: "/generated/image-a-male-people-ops-leader-in-a-startup-of.webp",
      testimonial: "Recruiting costs dropped sharply. Suna finds high-quality candidates so efficiently that it’s like having another team member."
    },
    {
      name: "Aliya Soliman, head of product at TripTrendr",
      position: undefined,
      imageSrc: "/generated/image-a-female-product-leader-in-a-travel-comp.webp",
      testimonial: "Market reports that took days now arrive in an hour. We avoid bad decisions and keep projects moving fast."
    }
  ]}
/>
<LogoScroller
	label="Trusted by industry leaders"
	logoUrls={[
		'https://logo.clearbit.com/zapier.com',
		'https://logo.clearbit.com/monday.com',
		'https://logo.clearbit.com/hubspot.com',
		'https://logo.clearbit.com/lever.co'
	]}
/>

<Summary
	title="Your AI employee for digital tasks"
	text="Suna by Kortix is a generalist AI Agent that autonomously completes research, recruiting, lead generation, trip planning, and more—so you focus on what matters most. 100% open source, transparent, and built for serious productivity."
/>




<Features
	title="Features"
	subtitle="Built for how you actually get work done."
	features={[
		{
			title: "100% open source",
			description: "Every line of code is public and auditable. No black box, no lock-in—just total transparency and control."
		},
		{
			title: "Truly autonomous agent",
			description: "Suna acts on your behalf to autonomously complete complex, multi-step tasks online, not just answer questions."
		},
		{
			title: "Works across any workflow",
			description: "From market research and lead generation to recruitment, trip planning, and SEO analysis—Suna adapts to your needs."
		},
		{
			title: "Stays up-to-date in real time",
			description: "Pulls fresh data and interacts with websites live—never works from stale or outdated information."
		},
		{
			title: "Runs anywhere you need it",
			description: "Choose cloud simplicity or self-host on your own infrastructure. Flexible deployment with zero barriers."
		},
		{
			title: "Flexible, open licensing",
			description: "Powered by the Apache 2.0 License, Suna is free for personal or business use—forever."
		}
	]}
/>

<UseCases
	title="Use Cases"
	subtitle="Real-world applications for your business needs"
	useCases={[
		{
			title: "Streamlined Workflows",
			description:
				"Automate repetitive tasks and connect systems to improve productivity with our industry-leading 87% time savings.",
			image:
				"https://images.unsplash.com/photo-1552664730-d307ca884978?ixlib=rb-4.0.3&ixid=MnwxMjA3fDB8MHxwaG90by1wYWdlfHx8fGVufDB8fHx8&auto=format&fit=crop&w=2940&q=80",
			link: {
				href: "/use-cases/workflows",
				label: "Learn more"
			}
		},
		{
			title: "Data Analysis",
			description:
				"Extract meaningful insights from your data with powerful analytical tools backed by proprietary AI algorithms that are 3x more accurate than competitors.",
			image:
				"https://images.unsplash.com/photo-1573496359142-b8d87734a5a2?ixlib=rb-4.0.3&ixid=MnwxMjA3fDB8MHxwaG90by1wYWdlfHx8fGVufDB8fHx8&auto=format&fit=crop&w=2488&q=80",
			link: {
				href: "/use-cases/data-analysis",
				label: "Explore analytics"
			}
		},
		{
			title: "Secure Collaboration",
			description:
				"Work together seamlessly while maintaining strict data privacy standards with our zero-knowledge architecture and military-grade encryption.",
			image:
				"https://images.unsplash.com/photo-1522202176988-66273c2fd55f?ixlib=rb-4.0.3&ixid=MnwxMjA3fDB8MHxwaG90by1wYWdlfHx8fGVufDB8fHx8&auto=format&fit=crop&w=2940&q=80",
			link: {
				href: "/use-cases/collaboration",
				label: "See security features"
			}
		}
	]}
/>

<AboutTeaser />
<CallToAction
  title="Your AI teammate, not just another tool"
  subtitle="Free up hours every week"
  description="Suna handles time-consuming digital work like lead research, candidate sourcing, and trip planning—independently, like a smart teammate who gets work done while you focus on the big picture. Suna is 100% open source and ready to join your team."
  callsToAction={[
    { href: "/get-started", label: "Start free", variant: "primary" },
    { href: "/pricing", label: "Explore pricing", variant: "secondary" },
    { href: "https://github.com/kortix-ai/suna", label: "View on GitHub", variant: "ghost" },
  ]}
  imageSrc="/generated/image-a-cheerful-business-professional-dressed.webp"
/>
