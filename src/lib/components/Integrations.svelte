<section class="py-24 bg-white">
  <div class="max-w-7xl mx-auto px-4 sm:px-6 lg:px-8">
    <div class="mb-12">
      <div class="text-xs font-semibold text-gray-500 uppercase tracking-wider mb-4">Supported providers</div>
      <h2 class="text-3xl font-semibold text-gray-900 mb-4">
        Works with all major UK credit cards and banks
      </h2>
      <p class="text-gray-500">Connect cards from any UK provider via secure Open Banking integration.</p>
      <a href="#" class="text-sm font-medium text-primary-600 hover:text-primary-700 flex items-center gap-1 mt-4">
        View all supported providers 
        <svg xmlns="http://www.w3.org/2000/svg" width="16" height="16" viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="2" stroke-linecap="round" stroke-linejoin="round"><path d="M5 12h14"></path><path d="m12 5 7 7-7 7"></path></svg>
      </a>
    </div>

    <div class="flex flex-wrap gap-4">
      {#each ['Barclays', 'HSBC', 'Lloyds', 'NatWest', 'Santander', 'TSB', 'Nationwide', 'Metro Bank', 'First Direct', 'Halifax'] as provider}
        <div class="px-6 py-4 bg-gray-50 rounded-xl flex items-center justify-center grayscale opacity-80 hover:grayscale-0 hover:opacity-100 transition-all duration-300">
           <span class="text-sm font-semibold text-gray-700">{provider}</span>
        </div>
      {/each}
    </div>
  </div>
</section>
