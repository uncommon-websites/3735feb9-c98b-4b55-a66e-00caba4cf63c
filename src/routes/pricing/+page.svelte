<script lang="ts">
	// Types
	import type { PageProps } from "./$types";

	// Components
	import Features from "$lib/components/layout/Features.svelte";
	import Testimonials from "$lib/components/layout/Testimonials.svelte";
	import CallToAction from "$lib/components/layout/CallToAction.svelte";
	import Pricing from "$lib/components/layout/Pricing.svelte";

	// Props
	const { data }: PageProps = $props();
</script>

<Pricing />

<Testimonials
  testimonials={[
    {
      name: "Javier Huang",
      position: "Operations Lead",
      company: "LinearNorth",
      quote:
        "We crunched the numbers—Suna saves us over 25 hours a month in research time. At $20, it basically pays for itself in a single automated task.",
      image: "/generated/image-a-professional-hispanic-man-in-a-dynamic.webp"
    },
    {
      name: "Marisol Dubois",
      position: "Digital Strategist",
      company: "Serenno Media",
      quote:
        "I was up and running the same afternoon. No learning curve, no integrations. It just worked—instantly started pulling backlinks for our SEO team.",
      image: "/generated/image-a-professional-french-woman-in-a-creativ.webp"
    },
    {
      name: "Celeste Ncube",
      position: "VP Sales Systems",
      company: "Cloudspire Labs",
      quote:
        "Suna has completely reshaped how our team operates. What used to take a sales admin an entire week now runs overnight with zero supervision.",
      image: "/generated/image-a-professional-black-woman-in-a-bustling.webp"
    }
  ]}
/>

<CallToAction
  title="The AI teammate that gets work done"
  subtitle="Focus on high-value work. Let Suna do the rest."
  description="Suna by Kortix is your autonomous AI agent, ready to handle research, lead generation, recruiting, travel plans, and more—without constant oversight. Skip repetitive tasks and start moving work forward. Get started free, or check out our open-source code on GitHub."
  imageSrc="/generated/image-a-cheerful-individual-sitting-at-a-woode.webp"
  callsToAction={[
    {
      href: '/signup',
      label: 'Get started free now',
      variant: 'primary'
    },
    {
      href: 'https://github.com/kortix-ai/suna',
      label: 'See it on GitHub',
      variant: 'secondary'
    }
  ]}
/>
