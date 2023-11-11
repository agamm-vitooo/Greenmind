<script>
  import img1 from '$lib/image/img1.jpg';
  import img2 from '$lib/image/img2.jpg';
  import img3 from '$lib/image/img3.jpg';
  
  let description = "Horem ipsum dolor sit amet, consectetur adipiscing elit.";

  let cards = [
    {
      imageSrc: img1,
      cardTitle: 'Natural Plants',
    },
    {
      imageSrc: img2,
      cardTitle: 'Plant Accessories',
    },
    {
      imageSrc: img3,
      cardTitle: 'Artificial Plants',
    },
  ];
</script>

<div class="container mx-auto mt-16 sm:mt-0 min-h-screen">
  <div class="text text-center mb-12">
    <div class="title text-stone-900 text-3xl font-bold">
      <h1>Categories</h1>
    </div>
    <div class="description text-stone-900 opacity-50">
      <h2>Find what you are looking for</h2>
    </div>
  </div>
  <div class="content flex flex-wrap justify-center">
    <div class="grid grid-cols-1 md:grid-cols-3 gap-8">
      {#each cards as card}
        <div class="rounded-lg text-center mx-auto px-10">
          <img src={card.imageSrc} alt={card.cardTitle} class="rounded-lg w-80 h-96 object-cover mx-auto mt-4" />
          <div class="p-4">
            <h3 class="text-xl font-semibold text-stone-900 mx-auto">{card.cardTitle}</h3>
          </div>
        </div>
      {/each}
    </div>
    <div class="text flex-wrap text-center mx-auto">
      <p class="text-center mb-3 text-stone-900 text-opacity-50 font-medium">{description}</p>
      <button class="btn bg-white border-white flex mx-auto items-center mb-16">
        Explore
        <script src="https://cdn.lordicon.com/lordicon-1.2.0.js"></script>
        <lord-icon
            src="https://cdn.lordicon.com/vduvxizq.json"
            trigger="hover"
            style="width:30px;height:30px">
        </lord-icon>
      </button>
    </div>
  </div>
</div>


<style>
  .content {
    background-color: #C1DCDC;
  }
</style>
