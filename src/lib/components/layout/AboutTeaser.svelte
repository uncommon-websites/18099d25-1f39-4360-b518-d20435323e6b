<!--
@component AboutTeaser
A minimalist teaser for the about page.
-->
<script lang="ts">
	// Types
	type TeamMember = {
		name: string;
		role: string;
		image: string;
	};

	// Components
	import Button from "../ui/Button.svelte";
	import ScrollText from "./sub/ScrollText.svelte";

	// State
	let sectionRef: HTMLElement;

	let props = $props();

	// Data
	const teamMember: TeamMember = {
		name: "Alex Morgan",
		role: "Founder & CEO",
		image: "/generated/image-medium-wide-editorial-documentary-portra.webp"
	};
</script>

<section bind:this={sectionRef} {...props}>
	<div class="section-px section-py container mx-auto">
		<div class="relative mx-auto grid max-w-2xl place-items-center gap-16">
			<ScrollText
				class="text-title1 text-center"
				text={`"I watched my parents spend six months trying to go solar—three contractors ghosted them, quotes made no sense, and they nearly gave up. That's when I realized the $400 billion solar industry had a coordination problem, not a technology problem. We're fixing it with voice agents and software that actually work."`}
			/>

			<!-- Team Member & CTA Section -->
			<div class="grid items-center gap-8 dark:border-gray-800">
				<div class="flex items-center justify-start gap-4">
					<img
						src={teamMember.image}
						alt={teamMember.name}
						class="size-12 rounded-full object-cover"
					/>
					<div>
						<div class="text-callout">{teamMember.name}</div>
						<div class="text-caption text-emphasis-low">{teamMember.role}</div>
					</div>
					<Button href="/about" variant="secondary" size="sm" class="ml-8">Read more</Button>
				</div>
			</div>
		</div>
	</div>
</section>
