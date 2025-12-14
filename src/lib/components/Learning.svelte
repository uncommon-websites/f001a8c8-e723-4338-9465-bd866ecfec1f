<section class="py-24 px-6 md:px-12 max-w-7xl mx-auto relative overflow-hidden bg-white">
	<div class="grid grid-cols-1 lg:grid-cols-2 gap-12 items-center relative z-10">
		<div>
			<span class="font-mono text-[10px] text-gray-500 uppercase tracking-widest mb-4 block">
				[ ADAPTIVE AI ]
			</span>
			<h2 class="font-display text-4xl md:text-5xl lg:text-6xl font-medium tracking-tight text-gray-900 mb-6 leading-[0.95]">
				AI That Learns<br>
				<span class="text-primary-500">Your Property</span>
			</h2>
			<p class="font-mono text-sm text-gray-600 max-w-md mb-8 leading-relaxed">
				HuntIQ's AI continuously learns from your property's unique patterns. Track deer sightings, log successful hunts, and watch predictions become more accurate with every season.
			</p>
			
			<a href="#early-access" class="bg-black text-white px-5 py-2.5 rounded text-sm font-medium hover:bg-gray-800 transition-colors inline-flex items-center gap-2 font-mono uppercase tracking-wide text-xs w-fit">
				<span class="text-primary-500">✦</span> See AI in Action
			</a>
		</div>

		<div class="relative h-[400px] w-full flex items-center justify-center">
			<!-- Background Text Pattern -->
            <div class="absolute inset-0 flex flex-col items-center justify-center opacity-5 select-none pointer-events-none overflow-hidden leading-none">
                {#each Array(10) as _, i}
                    <div class="text-6xl md:text-8xl font-black text-gray-900 whitespace-nowrap">
                        LEARNING LEARNING LEARNING
                    </div>
                {/each}
            </div>

            <!-- Floating Cards -->
            <div class="relative z-10 flex flex-col gap-4 w-full max-w-md">
                <div class="bg-white p-4 rounded shadow-lg border border-gray-200 transform -rotate-2 translate-x-4">
                    <div class="flex items-center gap-2 mb-2">
                        <span class="bg-primary-500 text-black text-[10px] font-bold px-1.5 py-0.5 rounded uppercase">AI Insight</span>
                        <span class="text-xs text-gray-500">Just now</span>
                    </div>
                    <p class="text-sm font-mono text-gray-800">Increased activity near creek crossing during cold fronts.</p>
                </div>

                <div class="bg-white p-4 rounded shadow-lg border border-gray-200 transform rotate-1 translate-x-8">
                    <div class="flex items-center gap-2 mb-2">
                        <span class="bg-primary-500 text-black text-[10px] font-bold px-1.5 py-0.5 rounded uppercase">AI Insight</span>
                        <span class="text-xs text-gray-500">2h ago</span>
                    </div>
                    <p class="text-sm font-mono text-gray-800">Thermal patterns favor north ridge stands in AM.</p>
                </div>

                 <div class="bg-white p-4 rounded shadow-lg border border-gray-200 transform -rotate-1">
                    <div class="flex items-center gap-2 mb-2">
                        <span class="bg-primary-500 text-black text-[10px] font-bold px-1.5 py-0.5 rounded uppercase">AI Insight</span>
                        <span class="text-xs text-gray-500">1d ago</span>
                    </div>
                    <p class="text-sm font-mono text-gray-800">Oak flat showing 3x higher movement this week.</p>
                </div>
            </div>
		</div>
	</div>
</section>
