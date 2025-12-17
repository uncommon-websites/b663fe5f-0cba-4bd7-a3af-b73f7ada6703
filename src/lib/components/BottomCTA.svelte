<script lang="ts">
  import Button from './ui/Button.svelte';
</script>

<section class="py-24 bg-white">
  <div class="max-w-7xl mx-auto px-4 sm:px-6 lg:px-8">
    <div class="relative rounded-3xl overflow-hidden h-[500px]">
      <img 
        src="/generated/image-diverse-group-of-happy-customers-in-thei-1766012832196-2.webp" 
        alt="Happy Incredible users" 
        class="absolute inset-0 w-full h-full object-cover"
      />
      <div class="absolute inset-0 bg-black/40"></div>
      
      <div class="absolute inset-0 flex flex-col justify-center px-8 md:px-16 max-w-3xl">
        <h2 class="text-4xl md:text-5xl font-bold text-white mb-8 leading-tight">
          Take control of your credit card payments today.
        </h2>
        <p class="text-xl text-white/90 mb-8">Join thousands of UK credit card holders who never miss a payment with Incredible.</p>
        <div class="flex flex-col sm:flex-row gap-4">
          <Button variant="primary" size="lg" class="rounded-full px-8">Get started free</Button>
          <Button variant="outline" size="lg" class="rounded-full px-8 bg-white text-gray-900 border-none hover:bg-gray-100">Book a demo</Button>
        </div>
      </div>
    </div>
  </div>
</section>
