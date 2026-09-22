<template>
  <section class="relative z-10 overflow-hidden bg-slate-50 pb-16 pt-20 lg:pb-24 lg:pt-28 text-slate-800">
    <div class="container mx-auto max-sm:px-6 lg:px-20">
      <div class="-mx-4 flex flex-wrap">
        <div class="w-full px-4">
          <div class="mx-auto mb-14 max-w-[550px] text-center" data-aos="fade-up">
            <span class="mb-2 block text-base font-semibold text-blue-600">
              Jangkauan Operasional
            </span>
            <h2 class="mb-4 text-3xl font-extrabold sm:text-4xl text-slate-900">
              Area Layanan Kami
            </h2>
            <p class="text-base text-slate-600">
              Kami siap meluncur cepat ke lokasi Anda dengan armada lengkap. Layanan tersedia 24 jam di kota:
            </p>
          </div>
        </div>
      </div>

      <div class="grid grid-cols-1 md:grid-cols-3 gap-6 max-w-5xl mx-auto">
        <!-- Surabaya -->
        <div class="w-full" data-aos="fade-up" data-aos-delay="0">
          <div class="group relative z-10 overflow-hidden rounded-2xl border border-slate-200/80 bg-white p-8 text-center shadow-sm transition-all duration-300 hover:-translate-y-2 hover:shadow-xl hover:border-blue-500">
            <div class="mx-auto mb-5 flex h-16 w-16 items-center justify-center rounded-2xl bg-blue-50 text-blue-600 transition-colors duration-300 group-hover:bg-blue-600 group-hover:text-white">
              <i class="bi bi-geo-alt-fill text-3xl"></i>
            </div>
            <h3 class="text-2xl font-bold text-slate-900 mb-2">Surabaya</h3>
            <p class="text-sm text-slate-500">Surabaya Pusat, Timur, Barat, Selatan & Utara</p>
            <div class="mt-4 pt-4 border-t border-slate-100 flex items-center justify-center gap-1 text-xs font-semibold text-blue-600">
              <i class="bi bi-truck"></i> Armada Siap Meluncur
            </div>
          </div>
        </div>

        <!-- Sidoarjo -->
        <div class="w-full" data-aos="fade-up" data-aos-delay="100">
          <div class="group relative z-10 overflow-hidden rounded-2xl border border-slate-200/80 bg-white p-8 text-center shadow-sm transition-all duration-300 hover:-translate-y-2 hover:shadow-xl hover:border-blue-500">
            <div class="mx-auto mb-5 flex h-16 w-16 items-center justify-center rounded-2xl bg-blue-50 text-blue-600 transition-colors duration-300 group-hover:bg-blue-600 group-hover:text-white">
              <i class="bi bi-geo-alt-fill text-3xl"></i>
            </div>
            <h3 class="text-2xl font-bold text-slate-900 mb-2">Sidoarjo</h3>
            <p class="text-sm text-slate-500">Waru, Gedangan, Candi, Porong, Krian, Sedati & Sekitarnya</p>
            <div class="mt-4 pt-4 border-t border-slate-100 flex items-center justify-center gap-1 text-xs font-semibold text-blue-600">
              <i class="bi bi-truck"></i> Armada Siap Meluncur
            </div>
          </div>
        </div>

        <!-- Gresik -->
        <div class="w-full" data-aos="fade-up" data-aos-delay="200">
          <div class="group relative z-10 overflow-hidden rounded-2xl border border-slate-200/80 bg-white p-8 text-center shadow-sm transition-all duration-300 hover:-translate-y-2 hover:shadow-xl hover:border-blue-500">
            <div class="mx-auto mb-5 flex h-16 w-16 items-center justify-center rounded-2xl bg-blue-50 text-blue-600 transition-colors duration-300 group-hover:bg-blue-600 group-hover:text-white">
              <i class="bi bi-geo-alt-fill text-3xl"></i>
            </div>
            <h3 class="text-2xl font-bold text-slate-900 mb-2">Gresik</h3>
            <p class="text-sm text-slate-500">Kebomas, Driyorejo, Menganti, Manyar & Sekitarnya</p>
            <div class="mt-4 pt-4 border-t border-slate-100 flex items-center justify-center gap-1 text-xs font-semibold text-blue-600">
              <i class="bi bi-truck"></i> Armada Siap Meluncur
            </div>
          </div>
        </div>
      </div>
    </div>
  </section>
</template>

<script setup>
</script>