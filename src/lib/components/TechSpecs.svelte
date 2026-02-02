<script lang="ts">
	// Technical specifications component
	const specs = [
		{
			category: "Sensor & Optics",
			items: [
				"Sony 4/3\" IMX sensor (400% larger than iPhone)",
				"Micro Four Thirds lens mount",
				"Compatible with 100+ professional lenses"
			]
		},
		{
			category: "AI Processing",
			items: [
				"Google Edge TPU AI chip",
				"Qualcomm Snapdragon SOC",
				"On-device neural network ISP pipeline",
				"Google Nano Banana AI integration"
			]
		},
		{
			category: "Software & OS",
			items: [
				"Camera Intelligence OS (custom Linux)",
				"Voice-controlled editing",
				"Real-time AI color grading",
				"Automatic corrections & denoising"
			]
		},
		{
			category: "Connectivity",
			items: [
				"Seamless iPhone integration",
				"4G/5G connectivity support",
				"Instant file transfer",
				"Cloud sync ready"
			]
		}
	];
</script>

<section class="w-full bg-gray-900 text-white py-20 md:py-32">
	<div class="max-w-7xl mx-auto px-6 md:px-8">
		<!-- Section Header -->
		<div class="text-center mb-16 md:mb-24">
			<h2 class="text-3xl md:text-5xl font-bold mb-4">
				Built Different
			</h2>
			<p class="text-lg md:text-xl text-gray-400 max-w-3xl mx-auto">
				Vertically-integrated AI-native technology stack designed from the ground up for intelligent content creation
			</p>
		</div>

		<!-- Specs Grid -->
		<div class="grid grid-cols-1 md:grid-cols-2 lg:grid-cols-4 gap-8 md:gap-12">
			{#each specs as spec}
				<div class="space-y-4">
					<h3 class="text-xl font-bold text-primary-400 uppercase tracking-wide">
						{spec.category}
					</h3>
					<ul class="space-y-3">
						{#each spec.items as item}
							<li class="text-gray-300 flex items-start">
								<svg class="w-5 h-5 text-primary-500 mr-2 mt-0.5 flex-shrink-0" fill="none" stroke="currentColor" viewBox="0 0 24 24">
									<path stroke-linecap="round" stroke-linejoin="round" stroke-width="2" d="M5 13l4 4L19 7" />
								</svg>
								<span>{item}</span>
							</li>
						{/each}
					</ul>
				</div>
			{/each}
		</div>

		<!-- Product Image -->
		<div class="mt-16 md:mt-24">
			<div class="max-w-4xl mx-auto">
				<img 
					src="/generated/image-small-business-owner-photographing-produ-1770061121713-4.webp" 
					alt="Caira camera in professional use"
					class="w-full h-auto rounded-lg shadow-2xl"
				/>
			</div>
		</div>
	</div>
</section>
