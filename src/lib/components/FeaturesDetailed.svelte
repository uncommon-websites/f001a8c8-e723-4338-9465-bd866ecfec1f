<script lang="ts">
	const features = [
		{
			iconPath: "M21 16V8a2 2 0 0 0-1-1.73l-7-4a2 2 0 0 0-2 0l-7 4A2 2 0 0 0 3 8v8a2 2 0 0 0 1 1.73l7 4a2 2 0 0 0 2 0l7-4A2 2 0 0 0 21 16z M3.3 7l8.7 5 8.7-5 M12 22.08V12",
			label: "AI-Powered Predictions",
			title: "Predictive deer movement modeling",
			description: "Our AI analyzes terrain features, food sources, bedding areas, and historical patterns to predict where deer will move throughout the day. Get probability heatmaps showing the most likely travel corridors and feeding areas."
		},
		{
			iconPath: "M12 2 L12 22 M12 2 L2 12 M12 2 L22 12",
			label: "Stand Placement",
			title: "Optimized stand recommendations",
			description: "HuntIQ recommends specific stand locations based on predicted deer movement, wind direction, access routes, and shooting lanes. Each recommendation includes confidence scores and optimal hunting times."
		},
		{
			iconPath: "M9.59 4.59A2 2 0 1 1 11 8H2m10.59 11.41A2 2 0 1 0 14 16H2m15.73-8.27A2.5 2.5 0 1 1 19.5 12H2",
			label: "Wind & Thermals",
			title: "Real-time wind and thermal modeling",
			description: "Advanced atmospheric modeling predicts wind patterns and thermal currents throughout your property. Know exactly how your scent will travel from any stand location at any time of day."
		},
		{
			iconPath: "M3 3 L21 21 M3 21 L21 3 M12 3 L12 21 M3 12 L21 12",
			label: "Access Routes",
			title: "Stealth access optimization",
			description: "AI-generated access routes minimize your scent footprint and noise signature. Get turn-by-turn directions that keep you downwind and hidden, maximizing your chance of an undetected approach."
		},
		{
			iconPath: "M3 3h18v18H3z M9 3v18 M3 9h18 M3 15h18 M15 3v18",
			label: "Terrain Analysis",
			title: "Property-level intelligence",
			description: "Deep terrain analysis identifies funnels, pinch points, saddles, and natural travel corridors. Our AI understands how topography influences deer behavior on your specific property."
		},
		{
			iconPath: "M22 12h-4l-3 9L9 3l-3 9H2",
			label: "Learning System",
			title: "Improves with every hunt",
			description: "HuntIQ learns from your observations and sightings. The more you use it, the more accurate predictions become. Your property intelligence compounds over time."
		}
	];
</script>

<section class="py-24 px-6 md:px-12 max-w-7xl mx-auto border-t border-gray-200 bg-white" id="features-detailed">
	<div class="text-center mb-16">
		<span class="font-mono text-[10px] text-gray-500 uppercase tracking-widest mb-4 block">
			[ KEY FEATURES ]
		</span>
		<h2 class="font-display text-4xl md:text-5xl font-medium tracking-tight text-gray-900 mb-4">
			Everything you need to hunt smarter
		</h2>
		<p class="font-mono text-sm text-gray-600 max-w-2xl mx-auto">
			HuntIQ combines advanced AI, real-time data, and property-specific intelligence to give you an unfair advantage in the field.
		</p>
	</div>

	<div class="grid grid-cols-1 md:grid-cols-2 lg:grid-cols-3 gap-8">
		{#each features as feature}
			<div class="group">
				<div class="mb-4 inline-flex items-center justify-center w-12 h-12 rounded-lg bg-gray-100 text-gray-900 transition-colors group-hover:bg-primary-500 group-hover:text-black">
					<svg xmlns="http://www.w3.org/2000/svg" width="24" height="24" viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="2" stroke-linecap="round" stroke-linejoin="round" class="w-6 h-6">
						<path d={feature.iconPath} />
					</svg>
				</div>
				
				<span class="font-mono text-[10px] text-gray-500 uppercase tracking-widest block mb-2">
					{feature.label}
				</span>
				
				<h3 class="font-display text-xl font-medium text-gray-900 mb-3">
					{feature.title}
				</h3>
				
				<p class="font-mono text-sm text-gray-600 leading-relaxed">
					{feature.description}
				</p>
			</div>
		{/each}
	</div>

	<div class="mt-16 text-center">
		<a href="#early-access" class="bg-primary-500 text-black px-6 py-3 rounded text-sm font-medium hover:bg-primary-600 transition-colors inline-flex items-center gap-2 font-mono uppercase tracking-wide">
			<svg viewBox="0 0 24 24" fill="none" xmlns="http://www.w3.org/2000/svg" width="16" height="16">
				<path d="M12 2L13.2 9.92154L20.6603 7L14.4 12L20.6603 17L13.2 14.0785L12 22L10.8 14.0785L3.33975 17L9.6 12L3.33975 7L10.8 9.92154L12 2Z" fill="currentColor" />
			</svg>
			Get Early Access
		</a>
	</div>
</section>
