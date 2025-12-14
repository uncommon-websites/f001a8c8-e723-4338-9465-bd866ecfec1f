<script lang="ts">
	import { slide } from 'svelte/transition';

	const faqs = [
		{
			question: "How does HuntIQ pricing work?",
			answer: "We're currently in beta and offering early access to select hunters. Pricing will be announced closer to our official launch. Beta users will receive special pricing."
		},
		{
			question: "What platforms does HuntIQ support?",
			answer: "HuntIQ will be available on iOS and Android mobile apps, plus a web dashboard for detailed planning. Offline mode ensures you can access your hunt plans without cell service."
		},
		{
			question: "Will my hunting spots be kept private?",
			answer: "Absolutely. Your property data and hunting locations are encrypted and never shared. We don't sell data or show your spots to other users. Your intelligence stays yours."
		},
		{
			question: "How accurate are the deer movement predictions?",
			answer: "Our AI combines terrain analysis, weather data, and historical patterns to generate predictions. Beta users report 70%+ accuracy on predicted movement corridors. Accuracy improves as the AI learns your specific property."
		},
		{
			question: "Do I need trail cameras to use HuntIQ?",
			answer: "No, HuntIQ works with terrain and weather data alone. However, trail camera integration is planned for future releases, which will further enhance prediction accuracy."
		},
		{
			question: "What property sizes does HuntIQ work best for?",
			answer: "HuntIQ is optimized for properties from 20 to 500+ acres. The AI adapts to your property size and provides relevant insights regardless of acreage."
		},
		{
			question: "How is HuntIQ different from OnX or Spartan Forge?",
			answer: "OnX and Spartan Forge provide maps and data. HuntIQ provides intelligence and decisions. We use AI to analyze your property and tell you where to hunt, not just where you are."
		},
		{
			question: "When will HuntIQ be available?",
			answer: "We're currently in closed beta. Join the waitlist to be notified when we open up more beta spots and for our official launch timeline."
		}
	];

	let openIndex: number | null = null;

	function toggle(index: number) {
		openIndex = openIndex === index ? null : index;
	}
</script>

<section class="py-24 px-6 md:px-12 max-w-7xl mx-auto border-t border-gray-200 bg-white" id="faq">
	<div class="grid grid-cols-1 lg:grid-cols-3 gap-12">
		<div>
			<span class="font-mono text-[10px] text-gray-500 uppercase tracking-widest mb-4 block">
				[ FAQ ]
			</span>
			<h2 class="font-display text-4xl md:text-5xl font-medium tracking-tight text-gray-900 mb-6">
				Frequently Asked Questions
			</h2>
			<p class="font-mono text-sm text-gray-600 mb-8">
				Your question not answered here?
			</p>
			<a href="mailto:hello@huntiq.ai" class="bg-primary-500 text-black px-5 py-2.5 rounded text-sm font-medium hover:bg-primary-600 transition-colors inline-flex items-center gap-2 font-mono uppercase tracking-wide text-xs">
				<svg xmlns="http://www.w3.org/2000/svg" width="14" height="14" viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="2" stroke-linecap="round" stroke-linejoin="round"><path d="M21 15a2 2 0 0 1-2 2H7l-4 4V5a2 2 0 0 1 2-2h14a2 2 0 0 1 2 2z"/></svg>
				Contact Us
			</a>
		</div>

		<div class="lg:col-span-2 space-y-4">
			{#each faqs as faq, i}
				<div class="border-b border-gray-200 pb-4">
					<button class="w-full flex items-center justify-between text-left py-2 group" on:click={() => toggle(i)}>
						<span class="font-mono text-sm font-medium text-gray-800 group-hover:text-primary-600 transition-colors pr-8">{faq.question}</span>
						<svg xmlns="http://www.w3.org/2000/svg" width="16" height="16" viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="2" stroke-linecap="round" stroke-linejoin="round" class="text-gray-400 transition-transform duration-300 {openIndex === i ? 'rotate-180' : ''}"><path d="m6 9 6 6 6-6"/></svg>
					</button>
					{#if openIndex === i}
						<div transition:slide={{ duration: 300 }} class="overflow-hidden">
							<p class="pt-2 pb-4 text-sm text-gray-600 leading-relaxed max-w-2xl font-mono">
								{faq.answer}
							</p>
						</div>
					{/if}
				</div>
			{/each}
		</div>
	</div>
</section>
