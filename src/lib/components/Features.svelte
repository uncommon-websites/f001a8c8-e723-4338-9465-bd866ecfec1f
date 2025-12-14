<script lang="ts">
	import FeatureCard from './FeatureCard.svelte';
</script>

<section class="py-24 px-6 md:px-12 max-w-7xl mx-auto relative bg-white" id="features">
    <!-- Background Grid Pattern -->
    <div class="absolute inset-0 z-0 opacity-30 pointer-events-none" 
        style="background-image: linear-gradient(#ccc 1px, transparent 1px), linear-gradient(90deg, #ccc 1px, transparent 1px); background-size: 40px 40px; mask-image: linear-gradient(to bottom, transparent, black 10%, black 90%, transparent);">
    </div>

	<div class="flex flex-col md:flex-row justify-between items-start md:items-end mb-16 gap-6 relative z-10">
		<div>
			<span class="font-mono text-[10px] text-gray-500 uppercase tracking-widest mb-4 block">
				[ CORE CAPABILITIES ]
			</span>
			<h2 class="font-display text-4xl md:text-5xl lg:text-6xl font-medium tracking-tight text-gray-900 mb-4">
				Intelligence, not just maps.
			</h2>
			<p class="font-mono text-sm text-gray-600 max-w-lg">
				HuntIQ delivers actionable predictions and optimized hunt plans using AI-powered terrain analysis.
			</p>
		</div>
		
		<a href="#early-access" class="bg-black text-white px-5 py-2.5 rounded text-sm font-medium hover:bg-gray-800 transition-colors flex items-center gap-2 font-mono uppercase tracking-wide text-xs">
			Get Early Access ->
		</a>
	</div>

	<div class="grid grid-cols-1 md:grid-cols-2 gap-6">
		<FeatureCard 
			subtitle="[ PREDICTIVE AI ]"
			title="Deer Movement<br>Heatmaps"
			description="AI-powered predictions show where deer are most likely to move based on terrain, wind, pressure, and historical patterns."
			tagColor="bg-primary-600"
			tagIcon="arrow"
            imageSrc="/generated/image-close-up-of-whitetail-deer-buck-in-natur-1765679114830-3.webp"
		/>
		
		<FeatureCard 
			subtitle="[ OPTIMIZED PLACEMENT ]"
			title="Smart Stand<br>Recommendations"
			description="Get AI-recommended stand locations that maximize your odds while accounting for wind direction and access routes."
			tagColor="bg-accent-orange"
			tagIcon="plus"
            imageSrc="https://placehold.co/600x400/1a1a1a/primary?text=Stand+Placement+Map"
		/>
		
		<FeatureCard 
			subtitle="[ WIND & THERMALS ]"
			title="Real-time Wind<br>Modeling"
			description="Advanced thermal and wind pattern predictions help you choose the perfect stand for current conditions."
			tagColor="bg-accent-yellow"
			tagIcon="arrow"
            imageSrc="https://placehold.co/600x400/1a1a1a/primary?text=Wind+Pattern+Visualization"
		/>
		
		<FeatureCard 
			subtitle="[ STEALTH ACCESS ]"
			title="Optimized Access<br>Routes"
			description="AI-generated routes minimize your scent footprint and noise, getting you to your stand undetected."
			tagColor="bg-primary-500"
			tagIcon="plus"
            imageSrc="/generated/image-hunter-walking-quietly-through-forest-at-1765679117244-4.webp"
		/>
	</div>
</section>
