<script>
  import Logo from './Logo.svelte';
</script>

<nav class="fixed top-0 left-0 right-0 z-50 bg-white/90 backdrop-blur-sm transition-all duration-300 border-b border-gray-100/50">
  <!-- Announcement Bar -->
  <div class="w-full py-2 text-center bg-white border-b border-gray-100 hidden md:block">
    <a href="#" class="text-[11px] font-medium text-gray-500 hover:text-gray-900 underline underline-offset-2 transition-colors">
      Watch Sierra Summit on-demand.
    </a>
  </div>

  <div class="max-w-[1400px] mx-auto px-6 h-20 flex items-center justify-between">
    <!-- Logo -->
    <div class="flex-shrink-0">
      <a href="/" class="flex items-center gap-2 text-sierra-green">
        <Logo className="w-8 h-8" />
        <span class="font-serif text-xl tracking-tight font-medium text-sierra-green">SIERRA</span>
      </a>
    </div>

    <!-- Navigation -->
    <div class="hidden md:flex items-center gap-8 text-sm font-medium text-gray-600">
      <a href="#" class="hover:text-gray-900 transition-colors">Product</a>
      <a href="#" class="hover:text-gray-900 transition-colors">Industries</a>
      <a href="#" class="hover:text-gray-900 transition-colors">Customers</a>
      <a href="#" class="hover:text-gray-900 transition-colors">Company</a>
    </div>

    <!-- Actions -->
    <div class="flex items-center gap-6 text-sm font-medium">
      <a href="#" class="text-gray-600 hover:text-gray-900 transition-colors">Sign in</a>
      <a href="#" class="bg-sierra-green hover:bg-sierra-green-hover text-white px-5 py-2.5 rounded-full transition-colors">
        Learn more
      </a>
    </div>
  </div>
</nav>
