<script>
  import Navbar from "../components/Navbar.svelte";
  import HeroSection from "../components/HeroSection.svelte";
  import ProductSection from "../components/ProductSection.svelte";
  import AboutSection from "../components/AboutSection.svelte";
  import CategoriesSection from "../components/CategoriesSection.svelte";
  import Footer from "../components/Footer.svelte";
</script>

<main class="scroll-smooth bg-white px-6 sm:px-16">
  <div data-aos="fade-up">
    <Navbar></Navbar>
    <HeroSection></HeroSection>
    <ProductSection></ProductSection>
    <AboutSection></AboutSection>
    <CategoriesSection></CategoriesSection>
    <Footer></Footer>

    <style>
      @import url('https://fonts.googleapis.com/css2?family=Poppins&display=swap');

      html{
        scroll-behavior: smooth;
      }
      main {
          font-family: 'Poppins', sans-serif;
      }
  </style>

</div>

</main>