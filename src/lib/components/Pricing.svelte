<script lang="ts">
	const plans = [
		{
			name: "Beta Access",
			price: "Free",
			period: "during beta",
			description: "Limited spots available for early adopters",
			features: [
				"Full access to core AI features",
				"Deer movement predictions",
				"Stand recommendations",
				"Wind & thermal modeling",
				"Access route optimization",
				"Property terrain analysis",
				"Priority support",
				"Lifetime discount when we launch"
			],
			cta: "Join Beta Waitlist",
			ctaLink: "#early-access",
			highlighted: true,
			badge: "Limited Spots"
		},
		{
			name: "Standard",
			price: "$19",
			period: "per month",
			description: "Perfect for hunters with 1-2 properties",
			features: [
				"Up to 2 properties",
				"AI deer movement predictions",
				"Stand placement recommendations",
				"Wind & thermal modeling",
				"Access route optimization",
				"Mobile app access",
				"Offline mode",
				"Email support"
			],
			cta: "Coming Soon",
			ctaLink: "#early-access",
			highlighted: false,
			badge: null
		},
		{
			name: "Pro",
			price: "$39",
			period: "per month",
			description: "For serious hunters and land managers",
			features: [
				"Unlimited properties",
				"Advanced AI predictions",
				"Historical pattern analysis",
				"Trail camera integration (coming soon)",
				"Multi-user property sharing",
				"Priority processing",
				"Advanced analytics dashboard",
				"Priority support"
			],
			cta: "Coming Soon",
			ctaLink: "#early-access",
			highlighted: false,
			badge: null
		}
	];
</script>

<section class="py-24 px-6 md:px-12 max-w-7xl mx-auto border-t border-gray-200 bg-white" id="pricing">
	<div class="text-center mb-16">
		<span class="font-mono text-[10px] text-gray-500 uppercase tracking-widest mb-4 block">
			[ PRICING ]
		</span>
		<h2 class="font-display text-4xl md:text-5xl font-medium tracking-tight text-gray-900 mb-4">
			Simple, transparent pricing
		</h2>
		<p class="font-mono text-sm text-gray-600 max-w-2xl mx-auto">
			Join our beta program for free access, or reserve your spot for launch pricing. No hidden fees, cancel anytime.
		</p>
	</div>

	<div class="grid grid-cols-1 md:grid-cols-3 gap-8 max-w-6xl mx-auto">
		{#each plans as plan}
			<div class={[
				'relative rounded-lg border p-8 transition-all',
				plan.highlighted ? 'border-primary-500 bg-gray-50' : 'border-gray-200 bg-white hover:border-gray-300'
			]}>
				{#if plan.badge}
					<div class="absolute -top-3 left-1/2 -translate-x-1/2">
						<span class="bg-primary-500 text-black px-3 py-1 rounded-full text-[10px] font-mono uppercase tracking-wide inline-flex items-center gap-1">
							<svg xmlns="http://www.w3.org/2000/svg" width="12" height="12" viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="2" stroke-linecap="round" stroke-linejoin="round" class="w-3 h-3">
								<polygon points="12 2 15.09 8.26 22 9.27 17 14.14 18.18 21.02 12 17.77 5.82 21.02 7 14.14 2 9.27 8.91 8.26 12 2"/>
							</svg>
							{plan.badge}
						</span>
					</div>
				{/if}

				<div class="mb-6">
					<h3 class="font-display text-2xl font-medium text-gray-900 mb-2">
						{plan.name}
					</h3>
					<p class="font-mono text-xs text-gray-600 mb-4">
						{plan.description}
					</p>
					<div class="flex items-baseline gap-1">
						<span class="font-display text-4xl font-medium text-gray-900">
							{plan.price}
						</span>
						<span class="font-mono text-sm text-gray-600">
							{plan.period}
						</span>
					</div>
				</div>

				<ul class="space-y-3 mb-8">
					{#each plan.features as feature}
						<li class="flex items-start gap-3">
							<div class="mt-0.5 flex-shrink-0">
								<svg xmlns="http://www.w3.org/2000/svg" width="16" height="16" viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="2" stroke-linecap="round" stroke-linejoin="round" class="w-4 h-4 text-primary-600">
									<polyline points="20 6 9 17 4 12"/>
								</svg>
							</div>
							<span class="font-mono text-xs text-gray-700">
								{feature}
							</span>
						</li>
					{/each}
				</ul>

				<a 
					href={plan.ctaLink} 
					class={[
						'block w-full text-center px-5 py-3 rounded text-sm font-medium transition-colors font-mono uppercase tracking-wide',
						plan.highlighted 
							? 'bg-primary-500 text-black hover:bg-primary-600' 
							: 'bg-gray-900 text-white hover:bg-gray-800'
					]}
				>
					{plan.cta}
				</a>
			</div>
		{/each}
	</div>

	<div class="mt-12 text-center">
		<p class="font-mono text-xs text-gray-500 mb-4">
			All plans include 14-day money-back guarantee after launch
		</p>
		<a href="#faq" class="text-sm text-primary-600 hover:text-primary-700 font-mono underline">
			Questions about pricing? Read our FAQ →
		</a>
	</div>
</section>
