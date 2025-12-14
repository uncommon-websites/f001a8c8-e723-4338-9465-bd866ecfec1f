<script lang="ts">
	// Stats
	const stats = [
		{ label: 'Acres Analyzed', value: '50K+' },
		{ label: 'Hunt Plans Generated', value: '2,500+' },
		{ label: 'Success Rate Increase', value: '3.2x' }
	];
</script>

<section class="relative pt-32 pb-16 px-6 md:px-12 max-w-7xl mx-auto min-h-screen flex flex-col justify-between bg-gradient-to-b from-black via-gray-950 to-black">
	<div class="grid grid-cols-1 lg:grid-cols-2 gap-12 items-center">
		<div class="z-10">
			<h1 class="text-6xl md:text-7xl lg:text-8xl font-display font-medium text-white leading-[0.9] tracking-tight mb-8">
				AI-Powered<br>
				<span class="text-primary-500">Hunt Intelligence</span>
			</h1>
			
			<div class="relative w-12 h-12 mb-8">
				<svg viewBox="0 0 24 24" fill="none" class="w-10 h-10 text-primary-500 absolute top-0 left-0">
					<path d="M12 2L13.2 9.92154L20.6603 7L14.4 12L20.6603 17L13.2 14.0785L12 22L10.8 14.0785L3.33975 17L9.6 12L3.33975 7L10.8 9.92154L12 2Z" fill="currentColor"/>
				</svg>
			</div>

			<div class="space-y-6 max-w-lg">
				<p class="font-mono text-sm text-gray-300 uppercase tracking-wider leading-relaxed">
					PREDICTIVE DEER MOVEMENT MODELING<br>
					AND OPTIMIZED STAND PLACEMENT<br>
					POWERED BY PROPERTY-LEVEL AI
				</p>

				<div class="flex flex-col items-start gap-3">
					<a href="#early-access" class="bg-primary-500 text-black px-6 py-3 rounded text-sm font-medium hover:bg-primary-600 transition-colors flex items-center gap-2 font-mono uppercase tracking-wide">
						Join Waitlist 
						<svg xmlns="http://www.w3.org/2000/svg" width="16" height="16" viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="2" stroke-linecap="round" stroke-linejoin="round"><path d="M5 12h14"/><path d="m12 5 7 7-7 7"/></svg>
					</a>
					<p class="text-[10px] text-gray-500 font-mono uppercase tracking-wide">
						Early access • Limited beta spots available
					</p>
				</div>
			</div>
		</div>

		<div class="relative h-[400px] lg:h-[600px] w-full flex items-center justify-center">
			<div class="absolute inset-0 flex items-center justify-center">
				<img src="/generated/image-a-serious-bowhunter-at-dawn-in-a-tree-st-1765679106137-0.webp" alt="Bowhunter at dawn" class="w-full h-full object-cover rounded-lg shadow-2xl" />
				<div class="absolute inset-0 bg-gradient-to-t from-black/60 via-transparent to-transparent rounded-lg"></div>
			</div>
		</div>
	</div>

	<div class="mt-20 border-t border-gray-800 pt-8">
		<div class="flex items-center gap-2 text-[10px] font-mono uppercase tracking-wider text-gray-500 mb-6">
			Trusted by serious whitetail hunters nationwide
		</div>
		
		<div class="grid grid-cols-3 gap-8">
			{#each stats as stat}
				<div class="flex flex-col">
					<span class="text-3xl md:text-4xl font-display font-medium text-primary-500 mb-1">{stat.value}</span>
					<span class="text-xs font-mono text-gray-400 uppercase tracking-wider">{stat.label}</span>
				</div>
			{/each}
		</div>
	</div>
</section>
