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
      name: "Michael Chen, head of growth at HiveLook",
      position: undefined,
      imageSrc: "/generated/image-a-professional-man-is-positioned-in-a-st.webp",
      testimonial: "Suna did three weeks of lead research in one day. I just dropped in a target account list and it handled the rest."
    },
    {
      name: "Laura Gómez, founder at Alta Bend",
      position: undefined,
      imageSrc: "/generated/image-a-confident-businesswoman-sits-at-her-de.webp",
      testimonial: "We needed to analyze over 20 competitors across multiple sites. Suna did the research and delivered a clean market report overnight."
    },
    {
      name: "Raj Patel, recruiter at Thread Partners",
      position: undefined,
      imageSrc: "/generated/image-a-businessman-is-comfortably-seated-in-h.webp",
      testimonial: "Sourcing candidates used to take hours of LinkedIn digging. Suna finds qualified profiles fast—with full context and links."
    },
    {
      name: "Sophie Tran, COO at Nomida Labs",
      position: undefined,
      imageSrc: "/generated/image-a-young-woman-is-in-a-creative-workspace.webp",
      testimonial: "We planned an entire company offsite in Lisbon—flights, hotels, co-working—all in one run. Suna just figured it out."
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
	generating
	title="What we do"
	text="Our technology delivers measurable results through secure, adaptable solutions that directly increase productivity and drive growth."
/>




<Features
	generating
	title="Features"
	subtitle="Some features"
	features={[
		{
			title: "Streamlined Workflows",
			description:
				"Automate repetitive tasks and connect systems to improve productivity with our industry-leading 87% time savings."
		},
		{
			title: "Data Analysis",
			description:
				"Extract meaningful insights from your data with powerful analytical tools backed by proprietary AI algorithms that are 3x more accurate than competitors."
		},
		{
			title: "Secure Collaboration",
			description:
				"Work together seamlessly while maintaining strict data privacy standards with our zero-knowledge architecture and military-grade encryption."
		}
	]}
/>

<UseCases
	generating
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

<AboutTeaser generating />
<CallToAction generating />
