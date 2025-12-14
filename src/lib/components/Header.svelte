<script lang="ts">
	import { onMount } from 'svelte';
	
	let isScrolled = false;

	onMount(() => {
		const handleScroll = () => {
			isScrolled = window.scrollY > 20;
		};
		window.addEventListener('scroll', handleScroll);
		return () => window.removeEventListener('scroll', handleScroll);
	});
</script>

<header class="fixed top-0 left-0 right-0 z-50 transition-all duration-300 px-6 py-4 flex items-center justify-between {isScrolled ? 'bg-black/90 backdrop-blur-md border-b border-gray-800' : 'bg-transparent'}">
	<div class="flex items-center gap-8">
		<a href="/" class="flex items-center gap-2 text-white font-medium text-xl tracking-tight">
			<div class="w-6 h-6 text-primary-500">
				<svg viewBox="0 0 24 24" fill="none" xmlns="http://www.w3.org/2000/svg">
					<path d="M12 2L13.2 9.92154L20.6603 7L14.4 12L20.6603 17L13.2 14.0785L12 22L10.8 14.0785L3.33975 17L9.6 12L3.33975 7L10.8 9.92154L12 2Z" fill="currentColor" />
				</svg>
			</div>
			HuntIQ
		</a>
		
		<nav class="hidden md:flex items-center gap-6 text-sm font-medium text-gray-400">
			<a href="#features" class="hover:text-white transition-colors">Features</a>
			<a href="#vision" class="hover:text-white transition-colors">Vision</a>
			<a href="#faq" class="hover:text-white transition-colors">FAQ</a>
		</nav>
	</div>

	<div class="flex items-center gap-4">
		<a href="#early-access" class="text-sm font-medium text-black bg-primary-500 px-5 py-2.5 rounded hover:bg-primary-600 transition-colors shadow-sm font-mono uppercase tracking-wide text-xs">Join Waitlist</a>
	</div>
</header>
