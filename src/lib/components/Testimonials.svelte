<script lang="ts">
	// Testimonials component
	const testimonials = [
		{
			quote: "Caira could replace Adobe Lightroom for many photographers. The AI editing is incredibly intuitive.",
			author: "TechRadar",
			role: "Technology Review"
		},
		{
			quote: "Finally, a camera that understands what I want to create. The voice control is a game-changer.",
			author: "Tony Northrup",
			role: "Photography YouTuber"
		},
		{
			quote: "The workflow is seamless. From capture to Instagram in under a minute - that's revolutionary.",
			author: "Jimmy Cheng",
			role: "Professional Photographer"
		}
	];
</script>

<section class="w-full bg-gray-50 py-20 md:py-32">
	<div class="max-w-7xl mx-auto px-6 md:px-8">
		<!-- Section Header -->
		<div class="text-center mb-16 md:mb-24">
			<h2 class="text-3xl md:text-5xl font-bold text-gray-900 mb-4">
				Trusted by Creators
			</h2>
			<p class="text-lg md:text-xl text-gray-600 max-w-3xl mx-auto">
				Over 1,000+ pre-orders from creators who are ready for the future of photography
			</p>
		</div>

		<!-- Testimonials Grid -->
		<div class="grid grid-cols-1 md:grid-cols-3 gap-8 md:gap-12">
			{#each testimonials as testimonial}
				<div class="bg-white p-8 rounded-lg shadow-sm">
					<div class="mb-6">
						<svg class="w-10 h-10 text-primary-500" fill="currentColor" viewBox="0 0 24 24">
							<path d="M14.017 21v-7.391c0-5.704 3.731-9.57 8.983-10.609l.995 2.151c-2.432.917-3.995 3.638-3.995 5.849h4v10h-9.983zm-14.017 0v-7.391c0-5.704 3.748-9.57 9-10.609l.996 2.151c-2.433.917-3.996 3.638-3.996 5.849h3.983v10h-9.983z" />
						</svg>
					</div>
					<p class="text-gray-700 mb-6 leading-relaxed italic">
						"{testimonial.quote}"
					</p>
					<div>
						<p class="font-semibold text-gray-900">{testimonial.author}</p>
						<p class="text-sm text-gray-600">{testimonial.role}</p>
					</div>
				</div>
			{/each}
		</div>

		<!-- Creator Image -->
		<div class="mt-16 md:mt-24">
			<div class="max-w-2xl mx-auto">
				<img 
					src="/generated/image-happy-content-creator-smiling-while-hold-1770061123709-5.webp" 
					alt="Happy creator with Caira camera"
					class="w-full h-auto rounded-lg shadow-lg"
				/>
			</div>
		</div>
	</div>
</section>
