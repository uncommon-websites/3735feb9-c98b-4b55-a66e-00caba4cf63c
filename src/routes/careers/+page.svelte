<script lang="ts">
	// Types

	// Components
	import SectionHeader from "$lib/components/layout/SectionHeader.svelte";
	import Culture from "$lib/components/layout/Culture.svelte";
	import Testimonials from "$lib/components/layout/Testimonials.svelte";
	import SecondaryHero from "$lib/components/layout/hero-sections/SecondaryHero.svelte";
	import Card from "$lib/components/ui/Card.svelte";
	import JobList, { type JobOpening } from "./JobList.svelte";

	// Icons
	import IconBriefcase from "~icons/lucide/briefcase";
	import IconUsers from "~icons/lucide/users";
	import IconHeart from "~icons/lucide/heart";
	import IconGlobe from "~icons/lucide/globe";

	// Constants
	const SECTION_BASE_CLASSES = "section-py section-px container mx-auto";
	const GRADIENT_BG_CLASSES =
		"bg-gradient-to-br from-gray-50 to-gray-100 dark:from-gray-900 dark:to-gray-800";
	const ICON_CONTAINER_CLASSES =
		"bg-primary-50 text-primary-600 dark:bg-primary-950 dark:text-primary-400 flex items-center justify-center rounded-full";

	const benefits = [
		{
			title: "Flexible Work",
			description: "Remote-first with flexible hours that respect work-life balance.",
			icon: IconBriefcase
		},
		{
			title: "Growth Opportunities",
			description: "Continuous learning with mentorship and education stipends.",
			icon: IconUsers
		},
		{
			title: "Comprehensive Benefits",
			description: "Health coverage, retirement plans, and generous paid time off.",
			icon: IconHeart
		}
	];

	const openings: JobOpening[] = [
		// Engineering
		{
			title: "Senior Frontend Developer",
			department: "Engineering",
			location: "Remote",
			type: "Full-time",
			url: "#"
		},
		{
			title: "Backend Engineer",
			department: "Engineering",
			location: "Remote",
			type: "Full-time",
			url: "#"
		},
		{
			title: "Design Engineer",
			department: "Engineering",
			location: "Remote",
			type: "Full-time",
			url: "#"
		},

		// Design
		{
			title: "UX/UI Designer",
			department: "Design",
			location: "Remote",
			type: "Full-time",
			url: "#"
		},
		{
			title: "Product Designer",
			department: "Design",
			location: "Remote",
			type: "Full-time",
			url: "#"
		},

		// Product
		{
			title: "Product Manager",
			department: "Product",
			location: "Remote",
			type: "Full-time",
			url: "#"
		},
		{
			title: "Product Analyst",
			department: "Product",
			location: "Remote",
			type: "Full-time",
			url: "#"
		},

		// Marketing
		{
			title: "Marketing Specialist",
			department: "Marketing",
			location: "Remote",
			type: "Full-time",
			url: "#"
		},
		{
			title: "Content Strategist",
			department: "Marketing",
			location: "Remote",
			type: "Full-time",
			url: "#"
		},
		{
			title: "Social Media Manager",
			department: "Marketing",
			location: "Remote",
			type: "Full-time",
			url: "#"
		}
	];

	const employeeTestimonials = [
	{
		name: "Michael Chen",
		position: "Senior Engineer",
		company: "Engineering Team",
		quote:
			"What I value most is how everyone genuinely helps each other grow. Whether I’m pair-programming, brainstorming solutions, or mentoring a new hire, I always feel respected and challenged. The culture rewards curiosity and collaboration. I’ve never learned so much so quickly, all while balancing my personal life too.",
		image: "/generated/image-a-senior-asian-male-engineer-smiling-in-.webp"
	},
	{
		name: "Priya Sharma",
		position: "Product Designer",
		company: "Design Team",
		quote:
			"I get the freedom to propose new ideas, experiment, and actually see my designs ship. Feedback is constant but constructive. There’s real mentorship here, and I feel like my voice matters at every stage. It’s the most energizing place I’ve worked as a creative."
		,
		image: "/generated/image-a-south-asian-female-product-designer-se.webp"
	},
	{
		name: "Marcus Johnson",
		position: "Marketing Lead",
		company: "Marketing Team",
		quote:
			"I started as a marketing specialist and now lead the team. Every step of the way, leadership supported my growth and made advancement feel possible. The environment is fast-paced but never cutthroat. Different perspectives are valued, and I always feel included and heard.",
		image: "/generated/image-a-black-male-marketing-lead-participatin.webp"
	}
];

	const processSteps = [
		{
			step: 1,
			title: "Apply",
			description:
				"Submit your application through our careers portal with your resume and portfolio."
		},
		{
			step: 2,
			title: "Interview",
			description: "Meet with our team to discuss your experience, skills, and career aspirations."
		},
		{
			step: 3,
			title: "Welcome aboard",
			description: "Join our team and start your journey building the future with us."
		}
	];

	const values = [
		{
			icon: IconHeart,
			title: "Passion",
			description: "We're driven by a shared passion for innovation and excellence."
		},
		{
			icon: IconUsers,
			title: "Collaboration",
			description: "We believe in teamwork and collaboration to achieve great things."
		},
		{
			icon: IconGlobe,
			title: "Global Impact",
			description: "We're committed to making a positive impact on the world."
		}
	];
</script>

<!-- Hero Section -->

<SecondaryHero
	title="Shape the future of open AI"
	subtitle="Join a global, collaborative team building autonomous agents that work for everyone—together, in the open"
	imageSrc="/generated/image-a-diverse-team-collaborating-in-a-modern.webp"
/>

<!-- Why Join Us Section -->
<section class={SECTION_BASE_CLASSES}>
	<SectionHeader title="Why join us?" subtitle="Build real impact, shape next-gen automation, and grow with a world-class open-source team." />

	<div class="prose mx-auto md:max-w-2xl mt-12 text-lg">
		<ul>
			<li><strong>Ship impact, not slides:</strong> You’ll build a product that helps people instantly, every time they run it.</li>
			<li><strong>Lead how work gets automated:</strong> Generalist agents are just emerging. Help shape how the next class of tools works.</li>
			<li><strong>Work alongside a real open-source community:</strong> Everything we make is transparent and public—because great software deserves it.</li>
			<li><strong>Pick up serious engineering & research experience:</strong> You’ll collaborate at the edge of AI, UX automation, and ops reliability.</li>
			<li><strong>Flexible setup:</strong> Work remotely, move quickly, and contribute in the way that fits you best.</li>
		</ul>
	</div>
</section>

<!-- Culture Section -->
<section class={SECTION_BASE_CLASSES}>
	<SectionHeader title="Our culture" subtitle="Build openly, iterate quickly, and focus on outcomes" />
	<div class="prose mx-auto md:max-w-2xl mt-12 text-lg">
		<div>
			<h3>Bias to build</h3>
			<p>We prioritize working code, product velocity, and user feedback over abstractions or committees.</p>
		</div>
		<div>
			<h3>Openness by default</h3>
			<p>Suna is 100% open source. We design in the open, develop in public, and treat our community like teammates.</p>
		</div>
		<div>
			<h3>No ego, just execution</h3>
			<p>We care about sharp thinking, fast learning, and getting the job done—not titles or politics.</p>
		</div>
	</div>
</section>

<Testimonials testimonials={employeeTestimonials} />

<!-- Application Process -->
<section class={SECTION_BASE_CLASSES}>
	<SectionHeader title="Application process" subtitle="Simple, transparent, and tailored for builders" />
	<div class="prose mx-auto md:max-w-2xl mt-12 text-lg">
		<ol>
			<li><strong>Apply online:</strong> Submit a short intro, your resume or GitHub, and any projects you’re proud of.</li>
			<li><strong>Intro call:</strong> We’ll talk about your experience, interests, and answer questions.</li>
			<li><strong>Trial task:</strong> You’ll get a short real-world problem we’ve handled or are currently facing.</li>
			<li><strong>Final chat:</strong> Meet more of the team, align expectations, and if it’s a mutual match—we’re moving.</li>
		</ol>
		<p>We move fast (2–7 days per step), communicate directly over email, and let you know where things stand at every stage. All roles are remote and open to global contributors.</p>
	</div>
</section>
<!-- Current Openings Section -->
<section class={GRADIENT_BG_CLASSES}>
	<div class="section-px section-py container mx-auto grid w-full items-start lg:grid-cols-2">
		<SectionHeader title="Current openings" subtitle="Find your perfect role" />

		<JobList {openings} />
	</div>
</section>
