<script setup>
import NavBar from './components/NavBar.vue';
import Home from './components/Home.vue';
import Services from './components/Services.vue';
import VisionMission from './components/VisionMission.vue';
import AboutUs from './components/AboutUs.vue';
import ServiceArea from './components/ServiceArea.vue';
import ContactUs from './components/ContactUs.vue';
</script>

<template>
  <header>
    <NavBar/>
  </header>

  <main>
    <section>
      <Home />
    </section>
    <section>
      <AboutUs />
    </section>
    <section>
      <VisionMission />
    </section>
    <section>
      <Services />
    </section>
    <section>
      <ServiceArea />
    </section>
    <section>
      <ContactUs />
    </section>
  </main>

  <!-- Floating WhatsApp Action Button -->
  <aside class="fixed bottom-6 right-6 z-50 flex items-center">
    <a href="https://wa.me/6287810816155?text=Halo%2C%20saya%20butuh%20bantuan%20jasa%20saluran%20mampet%20%2F%20sedot%20WC." 
       target="_blank"
       rel="noopener"
       aria-label="Chat WhatsApp Kami"
       class="group relative flex items-center gap-2.5 rounded-full bg-emerald-600 py-3.5 px-5 text-white shadow-2xl shadow-emerald-950/40 transition-all duration-300 hover:bg-emerald-500 hover:-translate-y-1 hover:shadow-emerald-500/50">
      <span class="absolute -top-1 -right-1 flex h-3.5 w-3.5">
        <span class="animate-ping absolute inline-flex h-full w-full rounded-full bg-emerald-300 opacity-75"></span>
        <span class="relative inline-flex rounded-full h-3.5 w-3.5 bg-emerald-300"></span>
      </span>
      <i class="bi bi-whatsapp text-2xl leading-none"></i>
      <span class="font-bold text-sm hidden sm:inline-block">Hubungi Kami</span>
    </a>
  </aside>
</template>

<style scoped>

</style>
