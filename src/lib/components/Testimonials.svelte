<script lang="ts">
	const testimonials = [
		{
			quote: "HuntIQ completely changed how I hunt my property. The AI predicted a bedding area I never would have found on my own. Tagged my biggest buck there opening week.",
			author: "Mike T.",
			role: "Bowhunter • Wisconsin",
			image: "/generated/image-portrait-of-confident-hunter-in-modern-h-1765679119597-5.webp"
		},
		{
			quote: "As a land manager, I've scouted hundreds of properties. HuntIQ's terrain analysis is scary accurate. It's like having a decade of experience on every new property.",
			author: "Jason R.",
			role: "Land Manager • Iowa",
			image: "/generated/image-portrait-of-confident-hunter-in-modern-h-1765679119597-5.webp"
		},
		{
			quote: "The wind modeling alone is worth it. I used to guess on thermals. Now I know exactly which stand to hunt based on conditions. My success rate tripled.",
			author: "Brad M.",
			role: "Serious Hunter • Ohio",
			image: "/generated/image-portrait-of-confident-hunter-in-modern-h-1765679119597-5.webp"
		},
		{
			quote: "I was skeptical about AI for hunting, but HuntIQ proved me wrong. It's not replacing woodsmanship—it's amplifying it. Best tool I've added to my arsenal.",
			author: "Derek S.",
			role: "Bowhunter • Illinois",
			image: "/generated/image-portrait-of-confident-hunter-in-modern-h-1765679119597-5.webp"
		},
		{
			quote: "The access route feature is genius. I was spooking deer on my way to stands without realizing it. HuntIQ showed me better paths I never considered.",
			author: "Travis K.",
			role: "Property Owner • Missouri",
			image: "/generated/image-portrait-of-confident-hunter-in-modern-h-1765679119597-5.webp"
		},
		{
			quote: "HuntIQ saves me hours of scouting. The predictive heatmaps are incredibly accurate. I'm seeing more mature bucks than ever before.",
			author: "Ryan P.",
			role: "Serious Hunter • Kansas",
			image: "/generated/image-portrait-of-confident-hunter-in-modern-h-1765679119597-5.webp"
		},
        {
			quote: "Finally, a hunting app that's actually intelligent. OnX shows me where I am. HuntIQ tells me where I should be. Huge difference.",
			author: "Matt L.",
			role: "Bowhunter • Kentucky",
			image: "/generated/image-portrait-of-confident-hunter-in-modern-h-1765679119597-5.webp"
		},
        {
			quote: "The AI learns my property over time. Each season it gets better. It's like having a personal hunting consultant who never sleeps.",
			author: "Chris D.",
			role: "Land Manager • Indiana",
			image: "/generated/image-portrait-of-confident-hunter-in-modern-h-1765679119597-5.webp"
		}
	];
</script>

<section class="py-24 px-6 md:px-12 max-w-7xl mx-auto bg-gray-50">
	<div class="text-center mb-16">
		<span class="font-mono text-[10px] text-gray-500 uppercase tracking-widest mb-4 block">
			[ HUNTER TESTIMONIALS ]
		</span>
		<h2 class="font-display text-4xl md:text-5xl font-medium tracking-tight text-gray-900 mb-4">
			Trusted by Serious Hunters
		</h2>
		<p class="font-mono text-sm text-gray-600">
			See what hunters are saying about their experience with HuntIQ
		</p>
	</div>

	<div class="columns-1 md:columns-2 lg:columns-3 gap-6 space-y-6">
		{#each testimonials as t}
			<div class="bg-white p-6 rounded-lg border border-gray-200 shadow-sm break-inside-avoid hover:shadow-md transition-shadow">
				<p class="font-mono text-xs leading-relaxed text-gray-700 mb-6">
					"{t.quote}"
				</p>
				<div class="flex items-center justify-between border-t border-gray-100 pt-4">
					<div class="flex items-center gap-3">
						<img src={t.image} alt={t.author} class="w-8 h-8 rounded-full bg-gray-200 object-cover" />
						<div>
							<div class="text-xs font-bold text-gray-900">{t.author}</div>
							<div class="text-[10px] text-gray-500 font-mono">{t.role}</div>
						</div>
					</div>
					<svg viewBox="0 0 24 24" fill="none" xmlns="http://www.w3.org/2000/svg" class="w-5 h-5 text-primary-500">
						<path d="M12 2L13.2 9.92154L20.6603 7L14.4 12L20.6603 17L13.2 14.0785L12 22L10.8 14.0785L3.33975 17L9.6 12L3.33975 7L10.8 9.92154L12 2Z" fill="currentColor" />
					</svg>
				</div>
			</div>
		{/each}
	</div>
</section>
