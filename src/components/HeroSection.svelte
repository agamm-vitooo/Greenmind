<script>
  import Plant from '$lib/image/plant.png';
  import Left from '$lib/image/vector-left.png';
  import Right from '$lib/image/vector-right.png';

  export let title = "Buy your dream plants";
  export let description_1 = "50+ Species";
  export let description_2 = "100+ Customers";
</script>

  <div class="scroll-smooth container-hero rounded-2xl min-h-screen p-4 md:p-8 md:flex items-center justify-between flex-col md:flex-row relative">
    <div class="md:w-1/2 md:pr-8 relative z-10">
      <h1 class="font-extrabold text-black text-5xl sm:text-4xl md:text-6xl mb-6 md:mb-10">{title}</h1>
      <div class="w-full md:w-80 text-lg text-stone-500 flex flex-col md:flex-row justify-between md:gap-12">
        <h2>{description_1}</h2>
        <div class="w-16 md:w-px border border-stone-900 hidden md:block"></div>
        <h2>{description_2}</h2>
      </div>
      <div class="flex items-center mt-9">
        <div class="relative w-full max-w-xs">
          <input type="text" placeholder="What are you looking for?" class="input input-bordered bg-white w-full" />
          <div class="absolute right-4 top-1/2 transform -translate-y-1/2 bg-slate-300 p-1 rounded-lg">
            <script src="https://cdn.lordicon.com/lordicon-1.1.0.js"></script>
            <lord-icon
              src="https://cdn.lordicon.com/kkvxgpti.json"
              trigger="hover"
              style="width:25px;height:25px">
            </lord-icon>
          </div>
        </div>
      </div>
    </div>
    <img src={Left} alt="Vector-Left" class="relative top-48 sm:top-28 w-16 sm:w-44 bottom-56 sm:bottom-0">
    <div class="md:w-1/2 mt-4 md:mt-0 relative">
      <img src={Plant} alt="Hero" class="relative z-20 rounded-lg w-full md:w-[411px] h-auto md:h-[513.98px]" />
      <div class="rectangle z-0 absolute bottom-0 w-full md:w-96 h-44 md:h-96 bg-stone-900 rounded-tl-full rounded-tr-full rounded-bl-full"></div>
    </div>
    <img src={Right} alt="Vector-Right" class="relative w-8 sm:w-28 bottom-64 sm:bottom-32 left-56 sm:-left-28 right-0 sm:right-28">
  </div>


<style>
  .container-hero{
    background-color: #C1DCDC;
  }
</style>