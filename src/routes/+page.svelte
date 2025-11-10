<script lang="ts">
	// Components
	import Summary from "$lib/components/layout/Summary.svelte";
	import Features from "$lib/components/layout/Features.svelte";
	import Testimonials from "$lib/components/layout/Testimonials.svelte";
	import CallToAction from "$lib/components/layout/CallToAction.svelte";
	import AboutTeaser from "$lib/components/layout/AboutTeaser.svelte";
	import LogoScroller from "$lib/components/layout/LogoScroller.svelte";
	import Hero from "$lib/components/layout/hero-sections/Hero.svelte";
</script>

<Hero
	title="Solar installation made simple"
	subtitle="Voice-guided design and coordination that eliminates the confusion, paperwork, and delays."
	imageSrc="/generated/image-a-group-of-confident-homeowners-aged-35-.webp"
	centered={false}
/>
<LogoScroller
	label="Trusted by industry leaders"
	logoUrls={[
		'https://cdn.brandfetch.io/redfin.com/w/400/h/400/logo',
		'https://cdn.brandfetch.io/opendoor.com/w/400/h/400/logo',
		'https://cdn.brandfetch.io/lennar.com/w/400/h/400/logo',
		'https://cdn.brandfetch.io/sunnova.com/w/400/h/400/logo'
	]}
/>

<Summary
	title="How it works"
	text="We automate solar installation from start to finish. Our voice agents guide homeowners through system design while our software coordinates installers at 3x normal efficiency. What used to take months of confusion and paperwork now happens smoothly in weeks."
/>

<Testimonials
	testimonials={[
		{
			name: "Priya Anand",
			position: "Homeowner",
			company: "Mountain View, CA",
			quote:
				"The entire process took just 6 weeks instead of the 4-6 months my neighbors spent. The voice-guided system walked me through design choices in under an hour, and coordination was seamless. I saved $8,400 compared to traditional quotes.",
			image: "/generated/image-editorial-documentary-photograph-of-a-pr.webp"
		},
		{
			name: "Carlos Rivera",
			position: "Homeowner",
			company: "Austin, TX",
			quote:
				"After getting three confusing quotes from other companies, this was refreshingly simple. The voice agent explained every option clearly, the installers showed up exactly when promised, and I avoided the usual contractor runaround. Worth every penny for the peace of mind alone.",
			image: "/generated/image-editorial-documentary-image-of-a-profess.webp"
		},
		{
			name: "Keisha Thompson",
			position: "Homeowner",
			company: "Phoenix, AZ",
			quote:
				"I was skeptical about solar after hearing horror stories, but the risk disappeared completely. Fixed pricing from day one, real-time coordination updates, and installation finished in 3 weeks. My energy bills dropped 72% in the first month. This is how solar should work.",
			image: "/generated/image-editorial-documentary-photograph-of-a-pr.webp"
		}
	]}
/>

<Features
	title="Everything you need for a seamless solar installation"
	subtitle="From your first conversation to final activation, our technology handles the complexity so you don't have to."
	features={[
		{
			title: "Voice-guided system design",
			description:
				"Talk through your energy needs and roof details naturally while our AI instantly generates a custom solar system design. No confusing jargon or technical expertise required."
		},
		{
			title: "Instant transparent pricing",
			description:
				"Get clear, itemized quotes with federal tax credits and financing options calculated in real-time. No hidden fees or surprise costs."
		},
		{
			title: "Automated installer coordination",
			description:
				"Our software automatically schedules permits, inspections, and installation crews at 3x the efficiency of traditional solar companies. Your timeline stays on track."
		},
		{
			title: "Zero paperwork hassle",
			description:
				"We handle all permits, utility interconnections, and tax credit applications automatically through our software platform. You just sign digitally when needed."
		},
		{
			title: "Real-time progress tracking",
			description:
				"Watch every step from permit approval to panel activation through your personalized dashboard. Know exactly what's happening and when."
		},
		{
			title: "Vetted installer network",
			description:
				"Every installer in our network is background-checked, licensed, and rated by previous customers. Quality work backed by our performance guarantee."
		}
	]}
/>
<AboutTeaser />
<CallToAction
	title="Start your solar journey in minutes"
	subtitle="Not months"
	description="While traditional solar companies leave you waiting weeks for quotes and drowning in paperwork, our voice-guided system designs your custom solar installation in under an hour. Join hundreds of homeowners who escaped the confusion and got their systems installed 3x faster."
	imageSrc="/generated/image-editorial-documentary-style-image-of-a-c.webp"
	callsToAction={[
		{
			href: "/get-started",
			label: "Design your system now",
			variant: "primary"
		},
		{
			href: "/how-it-works",
			label: "See how it works",
			variant: "secondary"
		}
	]}
/>
