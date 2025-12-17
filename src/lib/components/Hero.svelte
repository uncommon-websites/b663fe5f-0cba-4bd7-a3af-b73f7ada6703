<script lang="ts">
  import Button from './ui/Button.svelte';
</script>

<section class="pt-32 pb-16 overflow-hidden">
  <div class="max-w-7xl mx-auto px-4 sm:px-6 lg:px-8">
    <div class="max-w-4xl mx-auto text-center mb-16">
      <h1 class="text-5xl md:text-6xl font-semibold tracking-tight text-gray-900 mb-6 leading-[1.1]">
        One payment for all your credit cards. Automated.
      </h1>
      <p class="text-xl text-gray-600 mb-10 max-w-2xl mx-auto leading-relaxed">
        Incredible consolidates your credit card payments into one simple monthly payment via secure Open Banking integration. Never miss a payment again.
      </p>
      <div class="flex flex-col sm:flex-row items-center justify-center gap-4">
        <Button variant="primary" size="lg" class="rounded-full px-8">Get started free</Button>
        <Button variant="outline" size="lg" class="rounded-full px-8">See how it works</Button>
      </div>
    </div>

    <!-- Trust Indicators -->
    <div class="mb-12">
      <p class="text-xs font-semibold text-gray-500 uppercase tracking-wider mb-6 text-center">Trusted by UK credit card holders managing £200B+ in debt</p>
      <div class="flex flex-wrap items-center justify-center gap-8 opacity-60 grayscale px-4">
        <div class="flex items-center gap-2 text-sm font-semibold">
          <svg class="w-5 h-5" viewBox="0 0 24 24" fill="currentColor"><path d="M12 2L2 7l10 5 10-5-10-5zm0 9l2.5-1.25L12 8.5l-2.5 1.25L12 11zm0 2.5l-5-2.5-5 2.5L12 22l10-8.5-5-2.5-5 2.5z"/></svg>
          FCA Regulated
        </div>
        <div class="flex items-center gap-2 text-sm font-semibold">
          <svg class="w-5 h-5" viewBox="0 0 24 24" fill="currentColor"><path d="M12 1L3 5v6c0 5.55 3.84 10.74 9 12 5.16-1.26 9-6.45 9-12V5l-9-4z"/></svg>
          256-bit Encryption
        </div>
        <div class="flex items-center gap-2 text-sm font-semibold">
          <svg class="w-5 h-5" viewBox="0 0 24 24" fill="currentColor"><path d="M12 2C6.48 2 2 6.48 2 12s4.48 10 10 10 10-4.48 10-10S17.52 2 12 2zm-2 15l-5-5 1.41-1.41L10 14.17l7.59-7.59L19 8l-9 9z"/></svg>
          Open Banking
        </div>
      </div>
    </div>

    <!-- Hero Image -->
    <div class="relative rounded-2xl overflow-hidden shadow-2xl bg-gray-100">
      <img 
        src="/generated/image-young-professional-in-casual-clothes-sit-1766012825959-0.webp" 
        alt="Person managing credit card payments" 
        class="w-full h-[600px] object-cover object-center"
      />
      
      <!-- Floating UI Elements -->
      <div class="absolute top-1/2 left-1/2 transform -translate-x-1/2 -translate-y-1/2 flex flex-col gap-4">
        <!-- Notification 1 -->
        <div class="bg-white/90 backdrop-blur-sm p-4 rounded-xl shadow-lg flex items-center gap-4 animate-in fade-in slide-in-from-bottom-4 duration-700">
          <div class="w-10 h-10 bg-primary-600 rounded-full flex items-center justify-center text-white">
            <svg xmlns="http://www.w3.org/2000/svg" width="20" height="20" viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="2" stroke-linecap="round" stroke-linejoin="round"><polyline points="20 6 9 17 4 12"></polyline></svg>
          </div>
          <div>
            <div class="text-sm font-semibold text-gray-900">Payment scheduled</div>
            <div class="text-xs text-gray-500">£450 to 3 cards on 15th Jan</div>
          </div>
        </div>

        <!-- Notification 2 -->
        <div class="bg-white/90 backdrop-blur-sm p-4 rounded-xl shadow-lg flex items-center gap-4 ml-12 animate-in fade-in slide-in-from-bottom-4 duration-1000 delay-300">
          <div class="w-10 h-10 bg-primary-600 rounded-full flex items-center justify-center text-white">
             <svg xmlns="http://www.w3.org/2000/svg" width="20" height="20" viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="2" stroke-linecap="round" stroke-linejoin="round"><path d="M22 11.08V12a10 10 0 1 1-5.93-9.14"></path><polyline points="22 4 12 14.01 9 11.01"></polyline></svg>
          </div>
          <div>
            <div class="text-sm font-semibold text-gray-900">All cards paid</div>
            <div class="text-xs text-gray-500">You saved £45 in late fees</div>
          </div>
        </div>
      </div>
    </div>
  </div>
</section>
