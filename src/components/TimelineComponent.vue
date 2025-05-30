<template>
  <div class="relative max-w-7xl w-full px-5 mx-auto bg-[#10101E] py-20 overflow-x-auto container-scroll">
    <div class="absolute top-1/2 left-0 transform -translate-y-1/2 w-full h-1.5 bg-blue-600 z-0 hidden md:block"></div>

    <div class="flex flex-col md:flex-row md:justify-between md:items-center gap-20 relative z-10">
      <div class="relative md:w-1/4 flex-shrink-0 text-center">
        <i class="fa-solid fa-school absolute -top-10 left-1/2 -translate-x-1/2 w-12 h-12 bg-blue-600 text-white rounded-full flex items-center justify-center text-xl z-10"></i>
        <div class="bg-white rounded-lg shadow-md p-6 transition-transform hover:scale-[1.02] mt-8">
          <h2 class="text-lg font-bold mb-2">Ensino Médio</h2>
          <small class="block text-gray-500 mb-4">Janeiro 2021 - Dezembro 2023</small>
          <p class="text-gray-800 leading-relaxed">
            Cursando o Ensino Médio na ETEC Pedro D'Arcádia Neto em Assis/SP.
          </p>
        </div>
      </div>

      <div class="relative md:w-1/4 flex-shrink-0 text-center">
        <i class="fa-solid fa-gears absolute -top-10 left-1/2 -translate-x-1/2 w-12 h-12 bg-blue-600 text-white rounded-full flex items-center justify-center text-xl z-10"></i>
        <div class="bg-white rounded-lg shadow-md p-6 transition-transform hover:scale-[1.02] mt-8">
          <h2 class="text-lg font-bold mb-2">Técnico em Mecânica</h2>
          <small class="block text-gray-500 mb-4">Janeiro 2021 - Dezembro 2023</small>
          <p class="text-gray-800 leading-relaxed">
            Realizando Curso Técnico em Mecânica na ETEC Pedro D'Arcádia Neto em Assis/SP.
          </p>
        </div>
      </div>

      <div class="relative md:w-1/4 flex-shrink-0 text-center">
        <i class="fa-solid fa-user-tie absolute -top-10 left-1/2 -translate-x-1/2 w-12 h-12 bg-blue-600 text-white rounded-full flex items-center justify-center text-xl z-10"></i>
        <div class="bg-white rounded-lg shadow-md p-6 transition-transform hover:scale-[1.02] mt-8">
          <h2 class="text-lg font-bold mb-2">Aprendiz Administrativo</h2>
          <small class="block text-gray-500 mb-4">Março 2023 - Janeiro 2025</small>
          <p class="text-gray-800 leading-relaxed">
            Atuação como Aprendiz/Auxiliar Administrativo do setor de RH/Departamento Pessoal na gigante do setor sucroalcooleiro Raízen, unidade de Tarumã/SP.
          </p>
        </div>
      </div>

      <div class="relative md:w-1/4 flex-shrink-0 text-center">
        <i class="fa-solid fa-code absolute -top-10 left-1/2 -translate-x-1/2 w-12 h-12 bg-blue-600 text-white rounded-full flex items-center justify-center text-xl z-10"></i>
        <div class="bg-white rounded-lg shadow-md p-6 transition-transform hover:scale-[1.02] mt-8">
          <h2 class="text-lg font-bold mb-2">Graduando em Análise e Desenvolvimento de Sistemas</h2>
          <small class="block text-gray-500 mb-4">Janeiro 2025 - Atualmente</small>
          <p class="text-gray-800 leading-relaxed">
            Realizando graduação em ADS, na Universidade de Marília (Unimar) em Marília/SP, com previsão de término do curso para Dezembo/2026.
          </p>
        </div>
      </div>

    </div>
  </div>
</template>

<style>
.container-scroll::-webkit-scrollbar {
  width: 100%;
}

.container-scroll::-webkit-scrollbar-track {
  background: #888;
  border-radius: 6px;
}

.container-scroll::-webkit-scrollbar-thumb {
  background-color: blue;
  border-radius: 6px;
  border: 2px solid #f0f0f0;
}
</style>