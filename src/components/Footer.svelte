<script>
  let sections = [
    {
      title: 'Services',
      links: [
        { text: 'Branding', href: '/' },
        { text: 'Design', href: '/' },
        { text: 'Marketing', href: '/' },
        { text: 'Advertisement', href: '/' }
      ]
    },
    {
      title: 'Company',
      links: [
        { text: 'About us', href: '/' },
        { text: 'Contact', href: '/' },
        { text: 'Jobs', href: '/' },
        { text: 'Press kit', href: '/' }
      ]
    },
    {
      title: 'Legal',
      links: [
        { text: 'Terms of use', href: '/' },
        { text: 'Privacy policy', href: '/' },
        { text: 'Cookie policy', href: '/' }
      ]
    }
  ];
</script>

<style>
  .footer {
    background-color: #C1DCDC;
  }
</style>

<footer class="footer p-10 bg-base-200 rounded-2xl mt-10 sm:mt-0">
  <div class="title">
    <div class="text-black text-lg font-normal font-['Quella']">GREENMIND </div>
    <div class="w-48 text-stone-900 text-opacity-50 text-lg font-medium font-['Poppins']">We help you find your dream plant</div>
  </div>

  {#each sections as { title, links }}
    <nav>
      <header class="footer-title text-black">{title}</header>
      {#each links as { text, href }}
        <a href={href} class="link link-hover">{text}</a>
      {/each}
    </nav>
  {/each}
</footer>
