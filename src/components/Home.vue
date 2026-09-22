<template>
    <section class="relative flex min-h-[100vh] w-full max-w-[100vw] flex-col justify-center overflow-hidden" id="hero-section">
        <!-- Background Slider (full image without zoom distortion) -->
        <transition name="fade" mode="out-in">
            <img :src="images[currentIndex]" :key="images[currentIndex]" alt="Layanan Sedot WC"
                class="h-full w-full object-cover object-center absolute inset-0 z-0" id="hero-image" />
        </transition>

        <!-- Modern Dark Gradient Overlay for Readability -->
        <div class="absolute inset-0 bg-gradient-to-r from-slate-950/95 via-slate-900/80 to-slate-950/40 z-[1]"></div>

        <!-- Hero Content -->
        <div class="relative z-[5] flex flex-col justify-center min-h-[100vh] py-24 px-6 sm:px-10 lg:px-20 max-w-4xl text-white">
            <div class="mb-4 inline-flex items-center gap-2 px-3.5 py-1.5 rounded-full bg-blue-600/30 backdrop-blur-md border border-blue-400/40 text-blue-200 text-xs sm:text-sm font-semibold tracking-wide w-fit">
                <i class="bi bi-patch-check-fill text-blue-400"></i>
                <span>LAYANAN PROFESIONAL • CEPAT • HIGIENIS</span>
            </div>

            <h1 class="text-4xl sm:text-5xl lg:text-6xl font-black uppercase leading-[1.15] tracking-tight text-white drop-shadow-md">
                Ahli Mampet & Sedot WC
            </h1>

            <p class="mt-4 text-base sm:text-lg text-slate-200 font-normal leading-relaxed text-justify sm:text-left max-w-2xl">
                Spesialis sedot WC, pelancaran saluran pipa mampet, wastafel, kamar mandi, dan kuras septic tank di area Surabaya, Sidoarjo, dan Gresik. Pengerjaan cepat, bersih, dan bergaransi tanpa bongkar berlebihan.
            </p>

            <div class="mt-7 flex flex-wrap items-center gap-4">
                <a href="https://wa.me/6287810816155?text=Halo%2C%20saya%20tertarik%20dengan%20layanan%20AHLI%20MAMPET%20DAN%20SEDOT%20WC."
                    target="_blank"
                    class="inline-flex items-center gap-2.5 px-6 py-3.5 font-bold text-sm sm:text-base bg-emerald-600 text-white hover:bg-emerald-500 hover:-translate-y-1 transition-all duration-300 rounded-full shadow-lg shadow-emerald-950/30">
                    <i class="bi bi-whatsapp text-xl"></i>
                    <span>Hubungi WhatsApp Sekarang</span>
                </a>
                <a href="tel:6282145300565" target="_blank"
                    class="inline-flex items-center gap-2.5 px-6 py-3.5 font-bold text-sm sm:text-base bg-white text-slate-900 hover:bg-slate-100 hover:-translate-y-1 transition-all duration-300 rounded-full shadow-lg">
                    <i class="bi bi-telephone-fill text-blue-600 text-lg"></i>
                    <span>Telepon Langsung</span>
                </a>
            </div>

            <!-- Value Highlights (Zero emojis, 100% Bootstrap Icons) -->
            <div class="mt-10 pt-6 border-t border-white/15 grid grid-cols-2 sm:grid-cols-4 gap-4 text-xs sm:text-sm text-slate-200">
                <div class="flex items-center gap-2">
                    <i class="bi bi-clock-history text-cyan-400 text-lg"></i>
                    <span>Respon 24 Jam</span>
                </div>
                <div class="flex items-center gap-2">
                    <i class="bi bi-tools text-cyan-400 text-lg"></i>
                    <span>Tanpa Bongkar Total</span>
                </div>
                <div class="flex items-center gap-2">
                    <i class="bi bi-shield-check text-cyan-400 text-lg"></i>
                    <span>Garansi Tuntas</span>
                </div>
                <div class="flex items-center gap-2">
                    <i class="bi bi-wallet2 text-cyan-400 text-lg"></i>
                    <span>Harga Transparan</span>
                </div>
            </div>
        </div>

        <!-- Slider Dots Indicator -->
        <div class="absolute bottom-6 right-6 sm:right-12 z-[5] flex items-center gap-2">
            <button v-for="(img, idx) in images" :key="idx"
                @click="currentIndex = idx"
                :class="['h-2.5 rounded-full transition-all duration-300', currentIndex === idx ? 'w-8 bg-blue-400' : 'w-2.5 bg-white/40 hover:bg-white/70']"
                :aria-label="`Slide ${idx + 1}`">
            </button>
        </div>
    </section>
</template>

<script setup>
import { ref, onMounted } from 'vue';

const images = [
  new URL('@/assets/images/homepage/plumbing-service-1.jpg', import.meta.url).href,
  new URL('@/assets/images/homepage/vector-truck.png', import.meta.url).href,
  new URL('@/assets/images/homepage/plumbing-service-2.png', import.meta.url).href,
  new URL('@/assets/images/homepage/vector-truck-2.jpg', import.meta.url).href,
];

const currentIndex = ref(0);

onMounted(() => {
    setInterval(() => {
        currentIndex.value = (currentIndex.value + 1) % images.length;
    }, 5000); // 5 detik
});
</script>

<style scoped>
.fade-enter-active,
.fade-leave-active {
    transition: opacity 1s ease;
}

.fade-enter-from,
.fade-leave-to {
    opacity: 0;
}
</style>