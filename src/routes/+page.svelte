<script lang="ts">
	import Header from '$lib/components/Header.svelte';
	import Hero from '$lib/components/Hero.svelte';
	import Features from '$lib/components/Features.svelte';
	import FeaturesDetailed from '$lib/components/FeaturesDetailed.svelte';
	import Pricing from '$lib/components/Pricing.svelte';
	import CodebaseContext from '$lib/components/CodebaseContext.svelte';
	import CustomContext from '$lib/components/CustomContext.svelte';
	import Learning from '$lib/components/Learning.svelte';
	import Results from '$lib/components/Results.svelte';
	import Security from '$lib/components/Security.svelte';
	import Testimonials from '$lib/components/Testimonials.svelte';
	import CTABottom from '$lib/components/CTABottom.svelte';
	import FAQ from '$lib/components/FAQ.svelte';
	import Footer from '$lib/components/Footer.svelte';
</script>

<Header />

<main>
	<Hero />
	<Features />
	<FeaturesDetailed />
	<Pricing />
	<CodebaseContext />
	<CustomContext />
	<Learning />
	<Results />
	<Security />
	<Testimonials />
	<CTABottom />
	<FAQ />
</main>

<Footer />

