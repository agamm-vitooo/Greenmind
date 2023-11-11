<script>
  import Group_1 from '$lib/image/Group 1.svg';
  import Group_2 from '$lib/image/Group 2.svg';
  import Group_3 from '$lib/image/Group 3.svg';

  let title = "About Us";
  let description = "Order now and appreciate the beauty of nature";
  
  let cards = [
    {
      imageSrc: Group_1,
      cardTitle: 'Large Assortment',
      cardDescription: 'we offer many different types of products with fewer variations in each category.',
    },
    {
      imageSrc: Group_2,
      cardTitle: 'Fast & Free Shipping',
      cardDescription: '4-day or less delivery time, free shipping and an expedited delivery option.',
    },
    {
      imageSrc: Group_3,
      cardTitle: '24/7 Support',
      cardDescription: 'answers to any business related inquiry 24/7 and in real-time.',
    },
  ];
</script>

<div class="min-h-screen bg-white md:p-12">
  <h2 class="text-3xl font-bold text-center mb-5 mt-12 text-stone-900">{title}</h2>
  <p class="text-center mb-10 text-stone-900 text-opacity-50 font-medium">{description}</p>
  
  <div class="grid grid-cols-1 md:grid-cols-3 gap-8">
    {#each cards as card}
      <div class="bg-white rounded-lg text-center">
        <img src={card.imageSrc} alt={card.cardTitle} class="w-24 h-24 object-cover rounded-full mx-auto mt-4" />
        <div class="p-4">
          <h3 class="text-xl font-semibold mb-2 text-stone-900">{card.cardTitle}</h3>
          <p class="text-stone-900 text-opacity-50">{card.cardDescription}</p>
        </div>
      </div>
    {/each}
  </div>
</div>
