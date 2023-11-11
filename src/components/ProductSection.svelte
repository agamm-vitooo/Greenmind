<script>
  import Pic_1 from '$lib/image/pic-1.jpeg';
  import Pic_2 from '$lib/image/pic-2.jpeg';
  import Pic_3 from '$lib/image/pic-3.jpeg';

  let sectionTitle = "Best Selling Plants";
  let sectionDescription = "Easiest way to a healthy life by buying your favorite plants";

  let products = [
    { name: "Natural Plants", description: "₱ 1,400.00", image: Pic_1 },
    { name: "Artificial Plants", description: "₱ 900.00", image: Pic_2 },
    { name: "Artificial Plants", description: "₱ 3,500.00", image: Pic_3 },
  ];
</script>

<div class="bg-white min-h-screen p-8 flex flex-col md:flex-row items-center justify-between">
  <div class="md:w-1/2 pr-8">
    <h2 class="text-3xl font-bold text-stone-900 mb-4">{sectionTitle}</h2>
    <p class="text-stone-900 text-opacity-50 mb-4">{sectionDescription}</p>
    <button class="btn border-white text-black flex items-center">
      See More
      <script src="https://cdn.lordicon.com/lordicon-1.1.0.js"></script>
      <lord-icon
        src="https://cdn.lordicon.com/vduvxizq.json"
        trigger="hover"
        style="width: 40px; height: 40px;"
      ></lord-icon>
    </button>
  </div>

  <div class="md:w-1/2 mt-4 md:mt-0">
    <div class="grid grid-cols-1 sm:grid-cols-2 md:grid-cols-3 lg:grid-cols-4 xl:grid-cols-4 gap-4">
      {#each products as product (product.name)}
        <div class="bg-white p-4 rounded md:w-5/6">
          <img src={product.image} alt={product.name} class="rounded-xl w-72 h-96 object-cover"/>
          <h3 class="text-xl font-semibold mb-2">{product.name}</h3>
          <p class="text-gray-600 mb-4">{product.description}</p>
        </div>
      {/each}
    </div>
  </div>
  
  
</div>

<style>
  .btn{
    background-color: #C1DCDC;
  }
</style>
