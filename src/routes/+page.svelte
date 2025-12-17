<script lang="ts">
  import Header from "$lib/components/Header.svelte";
  import Hero from "$lib/components/Hero.svelte";
  import Stats from "$lib/components/Stats.svelte";
  import Steps from "$lib/components/Steps.svelte";
  import FeatureSection from "$lib/components/FeatureSection.svelte";
  import CaseStudies from "$lib/components/CaseStudies.svelte";
  import Integrations from "$lib/components/Integrations.svelte";
  import Resources from "$lib/components/Resources.svelte";
  import BottomCTA from "$lib/components/BottomCTA.svelte";
  import Footer from "$lib/components/Footer.svelte";
</script>

<Header />

<main>
  <Hero />
  <Stats />
  <Steps />
  
  <!-- Feature 1: One consolidated payment -->
  <FeatureSection 
    title="One simple payment for all your credit cards"
    subtitle="AUTOMATED PAYMENT CONSOLIDATION"
    linkText="See how it works"
    bullets={[
      "Single monthly payment covers all your cards",
      "Automatic distribution across multiple cards",
      "Smart payment optimization to minimize interest",
      "Never miss a payment deadline again"
    ]}
  >
    <div slot="description">
      <p>Stop juggling multiple payment dates and amounts. Incredible consolidates everything into one automated monthly payment that covers all your credit cards.</p>
    </div>
    <div slot="visual" class="w-full h-full flex items-center justify-center">
      <!-- Payment consolidation visual -->
      <div class="bg-white rounded-xl shadow-lg p-6 w-[80%] max-w-sm relative">
        <div class="mb-4">
          <div class="text-xs text-gray-500 mb-2">Monthly payment</div>
          <div class="text-3xl font-bold text-gray-900">£450</div>
        </div>
        <div class="space-y-3">
          <div class="flex items-center justify-between p-3 bg-gray-50 rounded-lg">
            <div class="flex items-center gap-2">
              <div class="w-8 h-8 rounded bg-primary-600 flex items-center justify-center text-white text-xs font-bold">V</div>
              <div class="text-xs font-medium">Visa ****1234</div>
            </div>
            <div class="text-xs font-semibold">£180</div>
          </div>
          <div class="flex items-center justify-between p-3 bg-gray-50 rounded-lg">
            <div class="flex items-center gap-2">
              <div class="w-8 h-8 rounded bg-primary-600 flex items-center justify-center text-white text-xs font-bold">M</div>
              <div class="text-xs font-medium">Mastercard ****5678</div>
            </div>
            <div class="text-xs font-semibold">£170</div>
          </div>
          <div class="flex items-center justify-between p-3 bg-gray-50 rounded-lg">
            <div class="flex items-center gap-2">
              <div class="w-8 h-8 rounded bg-primary-600 flex items-center justify-center text-white text-xs font-bold">A</div>
              <div class="text-xs font-medium">Amex ****9012</div>
            </div>
            <div class="text-xs font-semibold">£100</div>
          </div>
        </div>
        
        <!-- Floating success badge -->
        <div class="absolute -right-8 top-10 bg-primary-600 text-white p-3 rounded-lg shadow-md flex items-center gap-2">
           <svg xmlns="http://www.w3.org/2000/svg" width="16" height="16" viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="2" stroke-linecap="round" stroke-linejoin="round"><polyline points="20 6 9 17 4 12"></polyline></svg>
           <div class="text-xs font-medium">All paid!</div>
        </div>
      </div>
    </div>
  </FeatureSection>

  <!-- Feature 2: Secure Open Banking -->
  <FeatureSection 
    title="Bank-level security with Open Banking"
    subtitle="SECURE & REGULATED"
    linkText="Learn about security"
    reversed={true}
    bullets={[
      "FCA regulated Open Banking integration",
      "256-bit encryption for all transactions",
      "Never store your banking credentials",
      "Two-factor authentication on every login"
    ]}
  >
    <div slot="description">
      <p>Your security is our priority. We use Open Banking technology regulated by the FCA, ensuring your financial data is protected with the same security standards as your bank.</p>
    </div>
    <div slot="visual" class="w-full h-full flex items-center justify-center">
       <!-- Security flow diagram -->
       <div class="flex flex-col items-center gap-4">
         <div class="bg-white p-4 rounded-lg shadow-sm border border-gray-100 w-64 flex items-center gap-3">
            <div class="w-8 h-8 bg-primary-100 rounded flex items-center justify-center text-primary-600">
              <svg xmlns="http://www.w3.org/2000/svg" width="16" height="16" viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="2" stroke-linecap="round" stroke-linejoin="round"><rect x="3" y="11" width="18" height="11" rx="2" ry="2"></rect><path d="M7 11V7a5 5 0 0 1 10 0v4"></path></svg>
            </div>
            <div class="text-sm">
               <div class="font-semibold">Encrypted Connection</div>
               <div class="text-xs text-gray-500">Bank-grade 256-bit encryption</div>
            </div>
         </div>
         <div class="h-8 w-px bg-gray-300"></div>
         <div class="bg-white p-4 rounded-lg shadow-sm border border-gray-100 w-64 flex items-center gap-3">
            <div class="w-8 h-8 bg-primary-100 rounded flex items-center justify-center text-primary-600">
              <svg xmlns="http://www.w3.org/2000/svg" width="16" height="16" viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="2" stroke-linecap="round" stroke-linejoin="round"><path d="M12 22s8-4 8-10V5l-8-3-8 3v7c0 6 8 10 8 10z"></path></svg>
            </div>
            <div class="text-sm">
               <div class="font-semibold">FCA Regulated</div>
               <div class="text-xs text-gray-500">Fully compliant Open Banking</div>
            </div>
         </div>
         <div class="h-8 w-px bg-gray-300"></div>
         <div class="bg-primary-50 p-2 rounded-full text-xs text-primary-600 font-medium px-4 border border-primary-100">
            Your data is safe
         </div>
       </div>
    </div>
  </FeatureSection>

  <!-- Feature 3: Smart payment optimization -->
  <FeatureSection 
    title="Intelligent payment optimization that saves you money"
    subtitle="SMART ALGORITHMS"
    linkText="Learn about optimization"
    bullets={[
      "Automatically prioritize high-interest cards",
      "Minimize total interest paid across all cards",
      "Optimize payment timing for maximum impact",
      "Track savings compared to manual payments"
    ]}
  >
    <div slot="description">
      <p>Our smart algorithms analyze your credit card balances and interest rates to optimize payment distribution, helping you pay off debt faster while minimizing interest charges.</p>
    </div>
    <div slot="visual" class="w-full h-full flex items-center justify-center">
       <!-- Payment optimization UI -->
       <div class="bg-white rounded-2xl shadow-lg p-4 w-64 space-y-4">
          <div class="flex items-center gap-3 p-2 bg-gray-50 rounded-lg">
             <div class="w-10 h-10 bg-primary-600 rounded-lg flex items-center justify-center text-white text-xs font-bold">1</div>
             <div>
                <div class="text-xs font-bold">High APR Card</div>
                <div class="text-[10px] text-gray-500">24.9% APR • Priority payment</div>
             </div>
          </div>
          <div class="flex items-center gap-3 p-2 bg-gray-50 rounded-lg">
             <div class="w-10 h-10 bg-primary-600 rounded-lg flex items-center justify-center text-white text-xs font-bold">2</div>
             <div>
                <div class="text-xs font-bold">Medium APR Card</div>
                <div class="text-[10px] text-gray-500">19.9% APR • Balanced payment</div>
             </div>
          </div>
          <div class="flex items-center gap-3 p-2 bg-gray-50 rounded-lg">
             <div class="w-10 h-10 bg-primary-600 rounded-lg flex items-center justify-center text-white text-xs font-bold">3</div>
             <div>
                <div class="text-xs font-bold">Low APR Card</div>
                <div class="text-[10px] text-gray-500">12.9% APR • Minimum payment</div>
             </div>
          </div>
          <div class="mt-4 p-3 bg-primary-50 rounded-lg border border-primary-100">
            <div class="text-xs font-semibold text-primary-900">Estimated savings</div>
            <div class="text-lg font-bold text-primary-600">£145/month</div>
          </div>
       </div>
    </div>
  </FeatureSection>

  <!-- Feature 4: Complete visibility -->
  <FeatureSection 
    title="Track your progress with complete visibility"
    subtitle="REAL-TIME INSIGHTS"
    linkText="View dashboard demo"
    reversed={true}
    bullets={[
      "See all your cards and balances in one place",
      "Track payment history and upcoming payments",
      "Monitor debt reduction progress over time",
      "Get alerts before payments are processed"
    ]}
  >
    <div slot="description">
      <p>Stay informed with a clear dashboard that shows all your credit cards, payment schedules, and progress toward becoming debt-free.</p>
    </div>
    <div slot="visual" class="w-full h-full flex items-center justify-center">
       <!-- Dashboard mockup -->
       <div class="bg-white rounded-xl shadow-lg w-[80%] overflow-hidden border border-gray-100">
          <div class="bg-gray-50 p-3 border-b border-gray-100">
             <div class="text-xs font-semibold text-gray-900">Your Dashboard</div>
          </div>
          <div class="p-6">
             <div class="mb-4">
                <div class="text-xs text-gray-500 mb-1">Total balance</div>
                <div class="text-2xl font-bold text-gray-900">£8,450</div>
                <div class="text-xs text-primary-600 font-medium">↓ £450 this month</div>
             </div>
             <div class="space-y-2 mb-4">
                <div class="flex justify-between items-center text-xs">
                   <span class="text-gray-500">Next payment</span>
                   <span class="font-semibold">15th Jan</span>
                </div>
                <div class="flex justify-between items-center text-xs">
                   <span class="text-gray-500">Amount</span>
                   <span class="font-semibold">£450</span>
                </div>
             </div>
             <div class="h-2 bg-gray-100 rounded-full overflow-hidden">
                <div class="h-full bg-primary-600 rounded-full" style="width: 35%"></div>
             </div>
             <div class="text-[10px] text-gray-500 mt-1">35% paid off</div>
          </div>
       </div>
    </div>
  </FeatureSection>

  <!-- Feature 5: Flexible and adaptable -->
  <FeatureSection 
    title="Flexible payments that adapt to your life"
    subtitle="COMPLETE CONTROL"
    linkText="See all features"
    bullets={[
      "Adjust payment amounts anytime",
      "Pause or skip a month if needed",
      "Add or remove cards instantly",
      "Change payment dates to match your income"
    ]}
  >
    <div slot="description">
      <p>Life changes, and your payment plan should too. Incredible gives you complete flexibility to adjust your payments, add new cards, or pause when you need to—all from your phone.</p>
    </div>
    <div slot="visual" class="w-full h-full flex items-center justify-center px-8">
       <!-- Flexibility chart -->
       <div class="w-full h-64 flex items-end justify-between gap-2">
          {#each [60, 60, 60, 40, 60, 60, 80, 60, 60, 60, 60, 60] as height}
             <div class="w-full bg-primary-100 rounded-t-sm relative group">
                <div style="height: {height}%" class="absolute bottom-0 w-full bg-primary-600 rounded-t-sm transition-all duration-500 group-hover:bg-primary-700"></div>
             </div>
          {/each}
       </div>
       <!-- Legend overlay -->
       <div class="absolute top-12 right-12 bg-white p-4 rounded-lg shadow-sm border border-gray-100 text-xs">
          <div class="flex justify-between gap-8 mb-2">
             <span class="flex items-center gap-2"><span class="w-2 h-2 rounded-full bg-primary-600"></span> Monthly payment</span>
             <span class="font-semibold">£450</span>
          </div>
          <div class="flex justify-between gap-8 mb-2">
             <span class="flex items-center gap-2"><span class="w-2 h-2 rounded-full bg-primary-300"></span> Adjusted month</span>
             <span class="font-semibold">£300</span>
          </div>
          <div class="text-[10px] text-gray-500 mt-2">
             Flexibility when you need it
          </div>
       </div>
    </div>
  </FeatureSection>

  <!-- Feature 6: Security and compliance -->
  <FeatureSection 
    title="Built for security, compliance, and trust"
    subtitle="REGULATED & SECURE"
    linkText="Security details"
    reversed={true}
    bullets={[
      "FCA regulated and fully compliant",
      "Open Banking security standards",
      "GDPR compliant data handling",
      "Regular security audits and penetration testing"
    ]}
  >
    <div slot="description">
      <p>We take your financial security seriously. Incredible is FCA regulated, uses Open Banking technology, and maintains the highest standards of data protection and compliance.</p>
    </div>
    <div slot="visual" class="w-full h-full flex items-center justify-center">
       <!-- Compliance badges -->
       <div class="grid grid-cols-2 gap-8">
          <div class="flex flex-col items-center gap-2 text-center">
            <div class="w-16 h-16 bg-primary-100 rounded-full flex items-center justify-center">
              <svg class="w-8 h-8 text-primary-600" viewBox="0 0 24 24" fill="currentColor"><path d="M12 2L2 7l10 5 10-5-10-5zm0 9l2.5-1.25L12 8.5l-2.5 1.25L12 11zm0 2.5l-5-2.5-5 2.5L12 22l10-8.5-5-2.5-5 2.5z"/></svg>
            </div>
            <div class="font-bold text-sm">FCA Regulated</div>
          </div>
          <div class="flex flex-col items-center gap-2 text-center">
            <div class="w-16 h-16 bg-primary-100 rounded-full flex items-center justify-center">
              <svg class="w-8 h-8 text-primary-600" viewBox="0 0 24 24" fill="currentColor"><path d="M12 1L3 5v6c0 5.55 3.84 10.74 9 12 5.16-1.26 9-6.45 9-12V5l-9-4z"/></svg>
            </div>
            <div class="font-bold text-sm">256-bit Encryption</div>
          </div>
          <div class="flex flex-col items-center gap-2 text-center">
            <div class="w-16 h-16 bg-primary-100 rounded-full flex items-center justify-center">
              <svg class="w-8 h-8 text-primary-600" viewBox="0 0 24 24" fill="currentColor"><path d="M12 2C6.48 2 2 6.48 2 12s4.48 10 10 10 10-4.48 10-10S17.52 2 12 2zm-2 15l-5-5 1.41-1.41L10 14.17l7.59-7.59L19 8l-9 9z"/></svg>
            </div>
            <div class="font-bold text-sm">GDPR Compliant</div>
          </div>
          <div class="flex flex-col items-center gap-2 text-center">
            <div class="w-16 h-16 bg-primary-100 rounded-full flex items-center justify-center">
              <svg class="w-8 h-8 text-primary-600" viewBox="0 0 24 24" fill="currentColor"><rect x="3" y="11" width="18" height="11" rx="2" ry="2"/><path d="M7 11V7a5 5 0 0 1 10 0v4"/></svg>
            </div>
            <div class="font-bold text-sm">Open Banking</div>
          </div>
       </div>
    </div>
  </FeatureSection>

  <CaseStudies />
  <Integrations />
  <Resources />
  <BottomCTA />
</main>

<Footer />

