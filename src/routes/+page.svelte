<script>
  import { onMount } from 'svelte';

  // SVGs
  const arrowUpIcon = `<svg xmlns="http://www.w3.org/2000/svg" width="24" height="24" viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="2" stroke-linecap="round" stroke-linejoin="round" class="w-5 h-5 text-white"><path d="m5 12 7-7 7 7"/><path d="M12 19V5"/></svg>`;
  const playIcon = `<svg xmlns="http://www.w3.org/2000/svg" width="24" height="24" viewBox="0 0 24 24" fill="currentColor" stroke="currentColor" stroke-width="2" stroke-linecap="round" stroke-linejoin="round" class="w-4 h-4"><polygon points="5 3 19 12 5 21 5 3"/></svg>`;
</script>

<div class="w-full bg-white">
  <!-- Hero Section -->
  <section class="pt-32 pb-20 px-6 md:pt-40 md:pb-32">
    <div class="max-w-[1200px] mx-auto">
      <div class="text-center max-w-4xl mx-auto mb-16">
        <h1 class="text-5xl md:text-[64px] leading-[1.1] font-medium tracking-tight text-gray-900 mb-6">
          CX automation without<br />hallucinations. <span class="block">Guaranteed.</span>
        </h1>
        <p class="text-xl md:text-[22px] leading-relaxed text-gray-600 max-w-2xl mx-auto">
          Purpose-built AI models that eliminate hallucinations through<br class="hidden md:block" />deterministic policy enforcement. Built by Microsoft AI veterans.
        </p>
      </div>

      <!-- Hero Card -->
      <div class="bg-[#F4F4F0] rounded-[40px] p-8 md:p-20 w-full aspect-[16/10] md:aspect-[16/9] relative flex flex-col items-center justify-center shadow-sm">
        
        <!-- Search Bar Simulation -->
        <div class="w-full max-w-2xl bg-white rounded-full p-2 pl-8 pr-2 shadow-[0_4px_20px_rgba(0,0,0,0.04)] border border-primary/20 flex items-center justify-between mb-12 transform transition-transform hover:scale-[1.01] duration-300">
          <span class="text-xl text-primary/70 font-light tracking-wide">I need to change my flight and hotel booking</span>
          <button class="bg-primary hover:bg-primary-hover transition-colors rounded-full w-10 h-10 flex items-center justify-center">
            {@html arrowUpIcon}
          </button>
        </div>

        <!-- Watch Video Button -->
        <button class="absolute bottom-12 md:bottom-16 flex items-center gap-2 bg-gray-900 hover:bg-gray-800 text-white px-5 py-2.5 rounded-full text-sm font-medium transition-all hover:shadow-lg">
          <span class="w-5 h-5 flex items-center justify-center bg-white/20 rounded-full">
            {@html playIcon}
          </span>
          See APT-1 in Action
        </button>
      </div>
    </div>
  </section>

  <!-- Logos Section -->
  <section class="py-16 border-b border-gray-100">
    <div class="max-w-[1200px] mx-auto px-6">
      <p class="text-center text-sm font-medium text-gray-500 mb-10 uppercase tracking-wide">Trusted by Enterprise CX Leaders</p>
      <div class="grid grid-cols-2 md:grid-cols-5 gap-y-12 gap-x-8 items-center justify-items-center opacity-40 grayscale hover:grayscale-0 hover:opacity-70 transition-all duration-500">
        <!-- Banking & Finance -->
        <div class="h-8 flex items-center"><span class="font-bold text-xl">Chase</span></div>
        <div class="h-8 flex items-center"><span class="font-bold text-xl">Capital One</span></div>
        <div class="h-8 flex items-center"><span class="font-bold text-xl">Stripe</span></div>
        <div class="h-8 flex items-center"><span class="font-bold text-xl">Affirm</span></div>
        <div class="h-8 flex items-center"><span class="font-bold text-xl">Robinhood</span></div>
        
        <!-- Retail & E-commerce -->
        <div class="h-8 flex items-center"><span class="font-bold text-xl">Target</span></div>
        <div class="h-8 flex items-center"><span class="font-bold text-xl">Nordstrom</span></div>
        <div class="h-8 flex items-center"><span class="font-bold text-xl">Sephora</span></div>
        <div class="h-8 flex items-center"><span class="font-bold text-xl">Shopify</span></div>
        <div class="h-8 flex items-center"><span class="font-bold text-xl">Instacart</span></div>

        <!-- Travel & Hospitality -->
        <div class="h-8 flex items-center"><span class="font-bold text-xl">Marriott</span></div>
        <div class="h-8 flex items-center"><span class="font-bold text-xl">Expedia</span></div>
        <div class="h-8 flex items-center"><span class="font-bold text-xl">United</span></div>
        <div class="h-8 flex items-center"><span class="font-bold text-xl">Airbnb</span></div>
        <div class="h-8 flex items-center"><span class="font-bold text-xl">Hilton</span></div>
      </div>
    </div>
  </section>

  <!-- Feature Section 1 -->
  <section class="py-24 px-6">
    <div class="max-w-[1200px] mx-auto">
      <div class="flex flex-col md:flex-row gap-16 items-start">
        <!-- Visual -->
        <div class="w-full md:w-1/2 bg-[#EBEBE6] rounded-[32px] aspect-square relative overflow-hidden group">
          <div class="absolute inset-0 flex items-center justify-center p-8">
            <!-- Chat Bubble -->
            <div class="bg-white rounded-2xl p-4 shadow-sm max-w-[80%] flex gap-4 items-start animate-in fade-in slide-in-from-bottom-4 duration-1000">
              <div class="w-10 h-10 rounded-full bg-primary/10 flex-shrink-0 flex items-center justify-center">
                <svg xmlns="http://www.w3.org/2000/svg" width="20" height="20" viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="2" class="text-primary"><path d="M12 2L13.2 9.92154L20.6603 7L14.4 12L20.6603 17L13.2 14.0785L12 22L10.8 14.0785L3.33975 17L9.6 12L3.33975 7L10.8 9.92154L12 2Z"/></svg>
              </div>
              <div>
                <div class="text-xs font-medium text-gray-500 mb-1">APT-1 Agent</div>
                <div class="text-lg leading-snug text-gray-900">
                  Processing refund per policy 3.2.1...
                </div>
                <div class="mt-2 text-xs text-green-600 flex items-center gap-1">
                  <svg xmlns="http://www.w3.org/2000/svg" width="12" height="12" viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="3"><polyline points="20 6 9 17 4 12"/></svg>
                  Policy compliant
                </div>
              </div>
            </div>
          </div>
          <button class="absolute bottom-6 left-6 w-10 h-10 bg-white rounded-full flex items-center justify-center shadow-sm hover:scale-105 transition-transform">
            <svg xmlns="http://www.w3.org/2000/svg" width="16" height="16" viewBox="0 0 24 24" fill="currentColor" stroke="none"><rect x="6" y="4" width="4" height="16"/><rect x="14" y="4" width="4" height="16"/></svg>
          </button>
        </div>

        <!-- Content -->
        <div class="w-full md:w-1/2 pt-8">
          <div class="flex justify-between items-start mb-6">
            <h2 class="text-4xl md:text-[40px] leading-tight font-medium text-gray-900 max-w-md">
              Zero hallucinations. Guaranteed.
            </h2>
            <span class="bg-gray-900 text-white px-3 py-1.5 rounded-full text-xs font-medium">APT-1 Model</span>
          </div>
          
          <p class="text-gray-600 text-lg mb-12 leading-relaxed">
            Our proprietary APT-1 model ranks #1 on agentic benchmarks. Purpose-built for CX, not a repackaged generic model.
          </p>

          <div class="space-y-10">
            <!-- Feature 1 -->
            <div class="flex gap-4">
              <div class="mt-1">
                <svg xmlns="http://www.w3.org/2000/svg" width="20" height="20" viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="2" stroke-linecap="round" stroke-linejoin="round" class="text-gray-900"><path d="M12 22s8-4 8-10V5l-8-3-8 3v7c0 6 8 10 8 10z"/></svg>
              </div>
              <div>
                <h3 class="font-medium text-gray-900 mb-2">Deterministic policy enforcement</h3>
                <p class="text-gray-600 text-sm leading-relaxed">
                  Eliminate hallucinations through structured reasoning and program synthesis. Your policies are always followed, guaranteed.
                </p>
              </div>
            </div>

            <!-- Feature 2 -->
            <div class="flex gap-4">
              <div class="mt-1">
                <svg xmlns="http://www.w3.org/2000/svg" width="20" height="20" viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="2" stroke-linecap="round" stroke-linejoin="round" class="text-gray-900"><polyline points="16 18 22 12 16 6"/><polyline points="8 6 2 12 8 18"/></svg>
              </div>
              <div>
                <h3 class="font-medium text-gray-900 mb-2">Correct API orchestration</h3>
                <p class="text-gray-600 text-sm leading-relaxed">
                  Complex multi-step workflows executed flawlessly. Guaranteed correct integration with your existing systems.
                </p>
              </div>
            </div>

            <!-- Feature 3 -->
            <div class="flex gap-4">
              <div class="mt-1">
                <svg xmlns="http://www.w3.org/2000/svg" width="20" height="20" viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="2" stroke-linecap="round" stroke-linejoin="round" class="text-gray-900"><path d="M21 16V8a2 2 0 0 0-1-1.73l-7-4a2 2 0 0 0-2 0l-7 4A2 2 0 0 0 3 8v8a2 2 0 0 0 1 1.73l7 4a2 2 0 0 0 2 0l7-4A2 2 0 0 0 21 16z"/><polyline points="3.27 6.96 12 12.01 20.73 6.96"/><line x1="12" y1="22.08" x2="12" y2="12"/></svg>
              </div>
              <div>
                <h3 class="font-medium text-gray-900 mb-2">Built by Microsoft AI veterans</h3>
                <p class="text-gray-600 text-sm leading-relaxed">
                  Founded by Dan Roth (former CVP of Conversational AI at Microsoft) and Dan Klein (UC Berkeley AI Professor, Microsoft Technical Fellow).
                </p>
              </div>
            </div>
          </div>
        </div>
      </div>
    </div>
  </section>

  <!-- Testimonial Section -->
  <section class="py-12 px-6">
    <div class="max-w-[1200px] mx-auto">
      <div class="bg-[#F4F4F0] rounded-[32px] p-12 md:p-16 relative">
        <div class="mb-8 font-bold text-lg">Major Travel Company</div>
        <blockquote class="text-2xl md:text-3xl font-medium leading-tight text-gray-900 mb-12 max-w-4xl">
          "Generic models kept hallucinating and violating our policies. Scaled Cognition's APT-1 model gave us the reliability we needed to automate at scale."
        </blockquote>
        <div class="flex items-center justify-between flex-wrap gap-6">
          <div class="flex items-center gap-4">
            <img src="https://i.pravatar.cc/100?img=33" alt="Sarah Chen" class="w-12 h-12 rounded-full object-cover" />
            <div>
              <div class="font-medium text-gray-900">Sarah Chen</div>
              <div class="text-sm text-gray-500">VP of Customer Experience</div>
            </div>
          </div>
          <a href="#" class="inline-flex items-center gap-2 bg-gray-900 hover:bg-gray-800 text-white px-5 py-2.5 rounded-full text-sm font-medium transition-colors">
            Read case study
            <svg xmlns="http://www.w3.org/2000/svg" width="16" height="16" viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="2" stroke-linecap="round" stroke-linejoin="round"><path d="m9 18 6-6-6-6"/></svg>
          </a>
        </div>
      </div>
    </div>
  </section>

  <!-- Feature Section 2 (Omnichannel deployment) -->
  <section class="py-24 px-6 bg-[#F9F9F9]">
    <div class="max-w-[1200px] mx-auto">
      <div class="flex flex-col md:flex-row gap-16 items-start">
        <!-- Visual -->
        <div class="w-full md:w-1/2 bg-white rounded-[32px] aspect-square relative flex items-center justify-center p-8 shadow-sm">
           <!-- Audio Wave Animation Simulation -->
           <div class="flex items-center gap-1.5 h-16">
             {#each Array(15) as _, i}
               <div class="w-1.5 bg-gray-200 rounded-full animate-pulse" style="height: {20 + Math.random() * 40}%; animation-delay: {i * 0.1}s"></div>
             {/each}
           </div>
           <div class="absolute bottom-6 left-6 flex gap-2">
             <button class="w-8 h-8 rounded-full bg-gray-100 flex items-center justify-center hover:bg-gray-200 text-gray-600">
               <svg xmlns="http://www.w3.org/2000/svg" width="12" height="12" viewBox="0 0 24 24" fill="currentColor" stroke="none"><polygon points="5 3 19 12 5 21 5 3"/></svg>
             </button>
             <button class="w-8 h-8 rounded-full bg-gray-100 flex items-center justify-center hover:bg-gray-200 text-gray-600">
               <svg xmlns="http://www.w3.org/2000/svg" width="12" height="12" viewBox="0 0 24 24" fill="currentColor" stroke="none"><polygon points="11 5 6 9 2 9 2 15 6 15 11 19 11 5"/><path d="M19.07 4.93a10 10 0 0 1 0 14.14M15.54 8.46a5 5 0 0 1 0 7.07"/></svg>
             </button>
           </div>
        </div>

        <!-- Content -->
        <div class="w-full md:w-1/2 pt-8">
          <div class="flex justify-between items-start mb-6">
            <h2 class="text-4xl md:text-[40px] leading-tight font-medium text-gray-900 max-w-md">
              Omnichannel deployment
            </h2>
            <span class="bg-[bg-gray-900] text-white px-3 py-1.5 rounded-full text-xs font-medium">Request Demo</span>
          </div>
          
          <p class="text-gray-600 text-lg mb-12 leading-relaxed">
            Voice, chat, and email support across all channels. Multi-lingual capabilities for global enterprises.
          </p>

          <div class="space-y-10">
            <!-- Feature 1 -->
            <div class="flex gap-4">
              <div class="mt-1">
                <svg xmlns="http://www.w3.org/2000/svg" width="20" height="20" viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="2" stroke-linecap="round" stroke-linejoin="round" class="text-gray-900"><path d="M22 16.92v3a2 2 0 0 1-2.18 2 19.79 19.79 0 0 1-8.63-3.07 19.5 19.5 0 0 1-6-6 19.79 19.79 0 0 1-3.07-8.67A2 2 0 0 1 4.11 2h3a2 2 0 0 1 2 1.72 12.84 12.84 0 0 0 .7 2.81 2 2 0 0 1-.45 2.11L8.09 9.91a16 16 0 0 0 6 6l1.27-1.27a2 2 0 0 1 2.11-.45 12.84 12.84 0 0 0 2.81.7A2 2 0 0 1 22 16.92z"/></svg>
              </div>
              <div>
                <h3 class="font-medium text-gray-900 mb-2">Omnichannel-ready from day one</h3>
                <p class="text-gray-600 text-sm leading-relaxed">
                  Deploy across voice, chat, and email channels. Low inference time cost with multi-lingual support for global customer bases.
                </p>
              </div>
            </div>

            <!-- Feature 2 -->
            <div class="flex gap-4">
              <div class="mt-1">
                <svg xmlns="http://www.w3.org/2000/svg" width="20" height="20" viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="2" stroke-linecap="round" stroke-linejoin="round" class="text-gray-900"><circle cx="12" cy="12" r="10"/><path d="M2 12h20"/></svg>
              </div>
              <div>
                <h3 class="font-medium text-gray-900 mb-2">Integrate with your existing stack</h3>
                <p class="text-gray-600 text-sm leading-relaxed">
                  Integrates with your support platforms. Model-agnostic framework works with APT-1 alone or combined with other models.
                </p>
              </div>
            </div>

            <!-- Feature 3 -->
            <div class="flex gap-4">
              <div class="mt-1">
                <svg xmlns="http://www.w3.org/2000/svg" width="20" height="20" viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="2" stroke-linecap="round" stroke-linejoin="round" class="text-gray-900"><path d="M12 2v4"/><path d="m16.2 7.8 2.9-2.9"/><path d="M18 12h4"/><path d="m16.2 16.2 2.9 2.9"/><path d="M12 18v4"/><path d="m4.9 19.1 2.9-2.9"/><path d="M2 12h4"/><path d="m4.9 4.9 2.9 2.9"/></svg>
              </div>
              <div>
                <h3 class="font-medium text-gray-900 mb-2">PhD-level support for your team</h3>
                <p class="text-gray-600 text-sm leading-relaxed">
                  Direct access to our 20+ PhD-level researchers and engineers. We partner with you to achieve guaranteed outcomes at scale.
                </p>
              </div>
            </div>
          </div>
        </div>
      </div>
    </div>
  </section>

  <!-- Feature Section 3 (GenAPI™ development platform) -->
  <section class="py-24 px-6 bg-[#EBEBE6]">
    <div class="max-w-[1200px] mx-auto">
      <div class="flex flex-col md:flex-row gap-16 items-start">
        <!-- Visual -->
        <div class="w-full md:w-1/2 bg-[#DEDEd9] rounded-[32px] aspect-square relative flex items-center justify-center p-8 shadow-inner">
           <!-- Card Simulation -->
           <div class="bg-white rounded-2xl p-6 shadow-sm w-[80%] max-w-sm">
             <div class="flex gap-4 items-center mb-2">
               <div class="w-10 h-10 bg-[#E8DCC6] text-[#8B7355] rounded-full flex items-center justify-center text-xl font-serif font-bold">W</div>
               <div>
                 <div class="text-xs text-gray-500 uppercase tracking-wide font-medium">WestWalk Bags</div>
                 <div class="text-lg leading-snug text-gray-900">
                   Your order will arrive this Thursday.
                 </div>
               </div>
             </div>
           </div>
           
           <button class="absolute bottom-6 left-6 w-10 h-10 bg-white rounded-full flex items-center justify-center shadow-sm hover:scale-105 transition-transform">
             <svg xmlns="http://www.w3.org/2000/svg" width="16" height="16" viewBox="0 0 24 24" fill="currentColor" stroke="none"><rect x="6" y="4" width="4" height="16"/><rect x="14" y="4" width="4" height="16"/></svg>
           </button>
        </div>

        <!-- Content -->
        <div class="w-full md:w-1/2 pt-8">
          <div class="flex justify-between items-start mb-6">
            <h2 class="text-4xl md:text-[40px] leading-tight font-medium text-gray-900 max-w-md">
              GenAPI™ development platform
            </h2>
            <span class="bg-[bg-gray-900] text-white px-3 py-1.5 rounded-full text-xs font-medium">Our platform</span>
          </div>
          
          <p class="text-gray-600 text-lg mb-12 leading-relaxed">
            Build and train agents with simulated conversations. No-code, low-code, and pro-code SDKs for maximum flexibility.
          </p>

          <div class="space-y-4">
            <!-- Feature 1 (Active) -->
            <div class="bg-[#DEDEd9]/50 p-6 rounded-xl border border-transparent">
              <h3 class="font-medium text-gray-900 mb-2 text-sm">Simulated scenario-based training</h3>
              <p class="text-gray-600 text-xs leading-relaxed">
                GenAPI creates simulated conversations and scenarios for training. Copy Types enable natural language capability and rule setting.
              </p>
            </div>

            <!-- Feature 2 -->
            <div class="p-6 rounded-xl border border-gray-200/50 hover:bg-white/50 transition-colors cursor-pointer">
              <h3 class="font-medium text-gray-500 mb-0 text-sm">Function Conditions for business logic</h3>
            </div>

            <!-- Feature 3 -->
            <div class="p-6 rounded-xl border border-gray-200/50 hover:bg-white/50 transition-colors cursor-pointer">
              <h3 class="font-medium text-gray-500 mb-0 text-sm">Insight Engine and Agent Scorecard</h3>
            </div>
          </div>
        </div>
      </div>
    </div>
  </section>

  <!-- Security Section -->
  <section class="py-24 px-6 bg-[#1A1A1A] text-white">
    <div class="max-w-[1200px] mx-auto">
      <div class="flex flex-col md:flex-row gap-16 items-start">
        <!-- Visual (Left) -->
        <div class="w-full md:w-1/2 bg-[#111111] rounded-[32px] aspect-square relative flex items-center justify-center p-8 border border-white/10">
           <div class="text-center">
             <div class="text-white/40 text-2xl mb-4 font-light">cake recipe?</div>
             <div class="inline-flex items-center gap-2 bg-[#F59E0B] text-black px-4 py-2 rounded-full font-medium">
               <svg xmlns="http://www.w3.org/2000/svg" width="16" height="16" viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="2" stroke-linecap="round" stroke-linejoin="round"><circle cx="12" cy="12" r="10"/><line x1="4.93" x2="19.07" y1="4.93" y2="19.07"/></svg>
               Off topic
             </div>
           </div>
           
           <button class="absolute bottom-6 left-6 w-10 h-10 bg-white/10 rounded-full flex items-center justify-center hover:bg-white/20 transition-colors text-white">
             <svg xmlns="http://www.w3.org/2000/svg" width="16" height="16" viewBox="0 0 24 24" fill="currentColor" stroke="none"><rect x="6" y="4" width="4" height="16"/><rect x="14" y="4" width="4" height="16"/></svg>
           </button>
        </div>

        <!-- Content (Right) -->
        <div class="w-full md:w-1/2 pt-8">
          <h2 class="text-4xl md:text-[40px] leading-tight font-medium text-white mb-6">
            Enterprise-grade security
          </h2>
          
          <p class="text-gray-400 text-lg mb-12 leading-relaxed">
            Deploy in VPC, on-premises, or fully hosted. SOC 2 compliant with stateless architecture. Personal data never leaves your enterprise.
          </p>

          <div class="divide-y divide-white/10 border-t border-b border-white/10">
            {#each ['Supervision', 'Secure integration', 'Auditing', 'Data governance', 'Privacy'] as item, i}
              <div class="py-4">
                <div class="flex justify-between items-center cursor-pointer group">
                  <h3 class="font-medium text-gray-300 group-hover:text-white transition-colors text-sm">{item}</h3>
                  {#if i === 0}
                  <p class="mt-2 text-gray-500 text-xs max-w-md">Built-in guardrails with real-time monitoring for policy violations and jailbreak attempts. Complete audit trails.</p>
                  {/if}
                </div>
              </div>
            {/each}
          </div>
        </div>
      </div>
  </section>

  <!-- Results Section -->
  <section class="py-24 px-6">
    <div class="max-w-[1200px] mx-auto">
      <div class="flex justify-between items-end mb-16">
        <div class="max-w-xl">
          <h2 class="text-4xl md:text-[40px] leading-tight font-medium text-gray-900 mb-6">
            Proven results across industries
          </h2>
          <p class="text-gray-600 text-lg leading-relaxed">
            Scaled Cognition delivers higher automation rates and guaranteed policy compliance across banking, retail, and travel.
          </p>
        </div>
        <span class="bg-[bg-gray-900] text-white px-3 py-1.5 rounded-full text-xs font-medium mb-2">Our customers</span>
      </div>

      <div class="grid md:grid-cols-3 gap-8">
        <!-- Card 1: Sonos -->
        <div class="group cursor-pointer">
          <div class="relative aspect-square rounded-2xl overflow-hidden mb-6 bg-gray-100">
            <img src="https://images.unsplash.com/photo-1545454675-3531b543be5d?q=80&w=800&auto=format&fit=crop" alt="Sonos" class="w-full h-full object-cover transition-transform duration-500 group-hover:scale-105" />
            <div class="absolute inset-0 bg-black/20 group-hover:bg-black/10 transition-colors"></div>
            <div class="absolute top-1/2 left-1/2 -translate-x-1/2 -translate-y-1/2 text-white font-bold text-3xl tracking-widest">SONOS</div>
            <div class="absolute bottom-6 left-6 text-white">
              <div class="text-xs font-medium opacity-80 mb-1">Customers</div>
              <div class="text-2xl font-bold">15 Million</div>
            </div>
          </div>
          <h3 class="text-xl text-gray-900 leading-snug group-hover:text-[bg-gray-900] transition-colors">
            How Sonos elevates the listener experience with Sierra.
          </h3>
        </div>

        <!-- Card 2: SiriusXM -->
        <div class="group cursor-pointer">
          <div class="relative aspect-square rounded-2xl overflow-hidden mb-6 bg-gray-100">
            <img src="https://images.unsplash.com/photo-1550355291-bbee04a92027?q=80&w=800&auto=format&fit=crop" alt="SiriusXM" class="w-full h-full object-cover transition-transform duration-500 group-hover:scale-105" />
            <div class="absolute inset-0 bg-black/20 group-hover:bg-black/10 transition-colors"></div>
            <div class="absolute top-1/2 left-1/2 -translate-x-1/2 -translate-y-1/2 text-white font-bold text-3xl tracking-tighter">SiriusXM</div>
            <div class="absolute bottom-6 left-6 text-white">
              <div class="text-xs font-medium opacity-80 mb-1">Subscribers</div>
              <div class="text-2xl font-bold">34 Million</div>
            </div>
          </div>
          <h3 class="text-xl text-gray-900 leading-snug group-hover:text-[bg-gray-900] transition-colors">
            How SiriusXM increases listener loyalty with Sierra.
          </h3>
        </div>

        <!-- Card 3: Casper -->
        <div class="group cursor-pointer">
          <div class="relative aspect-square rounded-2xl overflow-hidden mb-6 bg-gray-100">
            <img src="https://images.unsplash.com/photo-1505693416388-b0346efee535?q=80&w=800&auto=format&fit=crop" alt="Casper" class="w-full h-full object-cover transition-transform duration-500 group-hover:scale-105" />
            <div class="absolute inset-0 bg-black/20 group-hover:bg-black/10 transition-colors"></div>
            <div class="absolute top-1/2 left-1/2 -translate-x-1/2 -translate-y-1/2 text-white font-serif text-3xl italic">Casper</div>
            <div class="absolute bottom-6 left-6 text-white w-full pr-6 flex justify-between">
              <div>
                <div class="text-xs font-medium opacity-80 mb-1">Resolution Rate</div>
                <div class="text-2xl font-bold flex items-center gap-1"><span class="text-sm">↗</span> 74%</div>
              </div>
              <div>
                <div class="text-xs font-medium opacity-80 mb-1">Increase in CSAT</div>
                <div class="text-2xl font-bold flex items-center gap-1"><span class="text-sm">↗</span> >20%</div>
              </div>
            </div>
          </div>
          <h3 class="text-xl text-gray-900 leading-snug group-hover:text-[bg-gray-900] transition-colors">
            How Casper turns a big purchase into a lifelong relationship with AI.
          </h3>
        </div>
      </div>
    </div>
  </section>

  <!-- CTA Section -->
  <section class="py-32 px-6 text-center">
    <div class="max-w-[1200px] mx-auto">
      <h2 class="text-4xl md:text-5xl font-medium text-gray-900 mb-6 tracking-tight">
        Ready to eliminate hallucinations?
      </h2>
      <p class="text-gray-600 text-lg max-w-2xl mx-auto mb-10">
        Join enterprise CX leaders who trust Scaled Cognition for guaranteed policy compliance and zero-hallucination automation.
      </p>
      <a href="#" class="inline-block bg-[bg-gray-900] hover:bg-[bg-gray-800] text-white px-8 py-3 rounded-full font-medium transition-colors">
        Request Demo
      </a>
    </div>
  </section>

  <!-- Footer -->
  <footer class="bg-[#F9F9F9] pt-20 pb-10 px-6 border-t border-gray-100">
    <div class="max-w-[1200px] mx-auto">
      <div class="grid grid-cols-2 md:grid-cols-6 gap-12 mb-20">
        <div class="col-span-2">
          <a href="/" class="flex items-center gap-2 text-[bg-gray-900] mb-6">
            <svg xmlns="http://www.w3.org/2000/svg" width="24" height="24" viewBox="0 0 24 24" fill="currentColor" class="w-6 h-6"><path d="M12 2L2 7l10 5 10-5-10-5zm0 9l2.5-1.25L12 8.5l-2.5 1.25L12 11zm0 2.5l-5-2.5-5 2.5L12 22l10-8.5-5-2.5-5 2.5z"/></svg>
            <span class="font-serif text-xl tracking-tight font-medium">SIERRA</span>
          </a>
        </div>
        
        <div>
          <h4 class="font-medium text-gray-900 mb-4 text-sm">Product</h4>
          <ul class="space-y-3 text-sm text-gray-600">
            <li><a href="#" class="hover:text-gray-900">Product overview</a></li>
            <li><a href="#" class="hover:text-gray-900">Meet your agent</a></li>
            <li><a href="#" class="hover:text-gray-900">Develop</a></li>
            <li><a href="#" class="hover:text-gray-900">Configure</a></li>
            <li><a href="#" class="hover:text-gray-900">Optimize</a></li>
            <li><a href="#" class="hover:text-gray-900">Assist</a></li>
            <li><a href="#" class="hover:text-gray-900">Voice</a></li>
            <li><a href="#" class="hover:text-gray-900">Trust and reliability</a></li>
          </ul>
        </div>

        <div>
          <h4 class="font-medium text-gray-900 mb-4 text-sm">Industries</h4>
          <ul class="space-y-3 text-sm text-gray-600">
            <li><a href="#" class="hover:text-gray-900">Industries overview</a></li>
            <li><a href="#" class="hover:text-gray-900">Financial services</a></li>
            <li><a href="#" class="hover:text-gray-900">Healthcare</a></li>
            <li><a href="#" class="hover:text-gray-900">Telecommunications</a></li>
            <li><a href="#" class="hover:text-gray-900">Media</a></li>
            <li><a href="#" class="hover:text-gray-900">Travel and hospitality</a></li>
            <li><a href="#" class="hover:text-gray-900">Retail and consumer goods</a></li>
            <li><a href="#" class="hover:text-gray-900">Technology</a></li>
          </ul>
        </div>

        <div>
          <h4 class="font-medium text-gray-900 mb-4 text-sm">Customers</h4>
          <ul class="space-y-3 text-sm text-gray-600">
            <li><a href="#" class="hover:text-gray-900">Customer stories</a></li>
          </ul>
        </div>

        <div>
          <h4 class="font-medium text-gray-900 mb-4 text-sm">Company</h4>
          <ul class="space-y-3 text-sm text-gray-600">
            <li><a href="#" class="hover:text-gray-900">About</a></li>
            <li><a href="#" class="hover:text-gray-900">Blog</a></li>
            <li><a href="#" class="hover:text-gray-900">Resources</a></li>
            <li><a href="#" class="hover:text-gray-900">Careers</a></li>
            <li><a href="#" class="hover:text-gray-900">Trust Center</a></li>
          </ul>
        </div>
      </div>

      <div class="flex flex-col md:flex-row justify-between items-center pt-8 border-t border-gray-200">
        <div class="flex flex-col md:flex-row items-center gap-6 mb-4 md:mb-0">
          <button class="bg-white border border-gray-200 rounded-md px-3 py-1.5 text-sm text-gray-600 flex items-center gap-2 hover:border-gray-300">
            United States (English)
            <svg xmlns="http://www.w3.org/2000/svg" width="12" height="12" viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="2" stroke-linecap="round" stroke-linejoin="round"><path d="m6 9 6 6 6-6"/></svg>
          </button>
          <div class="text-xs text-gray-500">
            © 2025 Sierra
            <a href="#" class="ml-4 hover:text-gray-900">Privacy Policy</a>
            <a href="#" class="ml-4 hover:text-gray-900">Terms & Conditions</a>
            <a href="#" class="ml-4 hover:text-gray-900">Cookie Preferences</a>
          </div>
        </div>

        <div class="flex items-center gap-4 text-gray-400">
          <a href="#" class="hover:text-gray-900"><svg xmlns="http://www.w3.org/2000/svg" width="20" height="20" viewBox="0 0 24 24" fill="currentColor"><path d="M16 8a6 6 0 0 1 6 6v7h-4v-7a2 2 0 0 0-2-2 2 2 0 0 0-2 2v7h-4v-7a6 6 0 0 1 6-6z"/><rect x="2" y="9" width="4" height="12"/><circle cx="4" cy="4" r="2"/></svg></a>
          <a href="#" class="hover:text-gray-900"><svg xmlns="http://www.w3.org/2000/svg" width="20" height="20" viewBox="0 0 24 24" fill="currentColor"><path d="M18.244 2.25h3.308l-7.227 8.26 8.502 11.24H16.17l-5.214-6.817L4.99 21.75H1.68l7.73-8.835L1.254 2.25H8.08l4.713 6.231zm-1.161 17.52h1.833L7.084 4.126H5.117z"/></svg></a>
          <a href="#" class="hover:text-gray-900"><svg xmlns="http://www.w3.org/2000/svg" width="20" height="20" viewBox="0 0 24 24" fill="currentColor"><path d="M22.54 6.42a2.78 2.78 0 0 0-1.94-2C18.88 4 12 4 12 4s-6.88 0-8.6.46a2.78 2.78 0 0 0-1.94 2A29 29 0 0 0 1 11.75a29 29 0 0 0 .46 5.33A2.78 2.78 0 0 0 3.4 19c1.72.46 8.6.46 8.6.46s6.88 0 8.6-.46a2.78 2.78 0 0 0 1.94-2 29 29 0 0 0 .46-5.33 29 29 0 0 0-.46-5.33zM9.75 15.02l5.75-3.27-5.75-3.27z"/></svg></a>
        </div>
      </div>
    </div>
  </footer>
</div>



