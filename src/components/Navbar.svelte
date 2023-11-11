<script>
  let isMobileMenuOpen = false;

  function toggleMobileMenu() {
    isMobileMenuOpen = !isMobileMenuOpen;
  }
</script>

<style>
  .nav-link {
    text-decoration: none;
    position: relative;
  }

  .nav-link:hover::before {
    content: '';
    position: absolute;
    bottom: -2px;
    left: 0;
    width: 100%;
    height: 2px;
    transition: ease-in-out 2.0;
    background-color: #000; /* Ganti dengan warna underlined yang Anda inginkan */
  }
</style>

<nav class="bg-white p-4 flex items-center justify-between sticky top-0 z-50">
  <div class="flex items-center">
    <div class="text-stone-900 text-2xl font-normal font-['Quella']">GREENMIND</div>
    <ul class="hidden md:flex ml-12 space-x-4 gap-8 text-stone-900 text-lg font-medium">
      <li><a class="nav-link" href="/">Home</a></li>
      <li><a class="nav-link" href="components/ProductSection.svelte">Product</a></li>
      <li><a class="nav-link" href="/contact">Contact</a></li>
    </ul>
  </div>

  <div class="md:hidden">
    <button on:click={toggleMobileMenu}>
      <svg class="w-6 h-6" fill="none" stroke="currentColor" viewBox="0 0 24 24" xmlns="http://www.w3.org/2000/svg">
        <path stroke-linecap="round" stroke-linejoin="round" stroke-width="2" d="M4 6h16M4 12h16M4 18h16"></path>
      </svg>
    </button>
  </div>

  <div class="hidden md:flex space-x-4">
    <script src="https://cdn.lordicon.com/lordicon-1.1.0.js"></script>
    <lord-icon
        src="https://cdn.lordicon.com/mfmkufkr.json"
        trigger="hover"
        style="width:30px;height:30px">
    </lord-icon>

    <script src="https://cdn.lordicon.com/lordicon-1.1.0.js"></script>
    <lord-icon
        src="https://cdn.lordicon.com/kthelypq.json"
        trigger="hover"
        style="width:30px;height:30px">
    </lord-icon>
  </div>
</nav>

{#if isMobileMenuOpen}
  <div class="md:hidden">
    <ul class="flex flex-col space-y-2 p-4">
      <div class="button flex gap-5">
        <script src="https://cdn.lordicon.com/lordicon-1.1.0.js"></script>
        <lord-icon
            src="https://cdn.lordicon.com/mfmkufkr.json"
            trigger="hover"
            style="width:30px;height:30px">
        </lord-icon>
    
        <script src="https://cdn.lordicon.com/lordicon-1.1.0.js"></script>
        <lord-icon
            src="https://cdn.lordicon.com/kthelypq.json"
            trigger="hover"
            style="width:30px;height:30px">
        </lord-icon>
      </div>
      <li><a class="nav-link" href="/">Home</a></li>
      <li><a class="nav-link" href="/ProductSection.svelte">Product</a></li>
      <li><a class="nav-link" href="/contact">Contact</a></li>
    </ul>
  </div>
{/if}

