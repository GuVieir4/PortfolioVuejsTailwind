<template>
  <section class="bg-[#10101E] py-16 px-4 min-h-screen flex items-center justify-center">
    <form ref="contactForm" @submit.prevent="enviarFormulario"
      class="max-w-2xl w-full bg-[#1A1A2E] p-8 rounded-lg shadow-lg space-y-6">
      
      <div class="text-center mb-6">
        <h2 class="text-4xl font-extrabold text-white mb-2">Contato</h2>
        <p class="text-gray-400 mt-5">Quer que eu entre em contato com você? Preencha o formulário abaixo.</p>
      </div>

      <div>
        <label for="name" class="block text-sm font-medium text-gray-300 mb-1">Nome</label>
        <div class="relative">
          <i class="fa-solid fa-user absolute top-1/2 left-3 -translate-y-1/2 text-blue-400"></i>
          <input type="text" id="name" name="name" placeholder="Seu nome" required
            class="pl-10 w-full px-4 py-2 bg-[#10101E] border border-blue-800 text-white rounded" />
        </div>
      </div>

      <div>
        <label for="email" class="block text-sm font-medium text-gray-300 mb-1">E-mail</label>
        <div class="relative">
          <i class="fa-solid fa-envelope absolute top-1/2 left-3 -translate-y-1/2 text-blue-400"></i>
          <input type="email" id="email" name="email" placeholder="seu@email.com" required
            class="pl-10 w-full px-4 py-2 bg-[#10101E] border border-blue-800 text-white rounded" />
        </div>
      </div>

      <div>
        <label for="message" class="block text-sm font-medium text-gray-300 mb-1">Mensagem</label>
        <textarea id="message" name="message" rows="5" placeholder="Digite sua mensagem..." required
          class="w-full px-4 py-2 bg-[#10101E] border border-blue-800 text-white rounded resize-none"></textarea>
      </div>

      <div class="text-center">
        <button type="submit" class="bg-[#010409] hover:bg-blue-800 text-white font-semibold py-2 px-6 rounded flex items-center justify-center gap-2 mx-auto">
          <i class="fa-solid fa-paper-plane"></i> Enviar </button>
          <p class="text-gray-400 mt-5">Obs: O formulário funciona!</p>
      </div>
    </form>
  </section>
</template>

<script>
export default {
  name: "FormularioContato",

  mounted() {
    if (window.emailjs) {
      window.emailjs.init("ox99hOXlUY7nMnKnS");
      console.log("EmailJS inicializado com sucesso!");
    } else {
      console.error("Erro: EmailJS não está funcionando.");
    }
  },

  methods: {
    enviarFormulario() {
      const formulario = this.$refs.contactForm;

      if (!window.emailjs) {
        alert("Erro: EmailJS não está funcionando.");
        return;
      }

      window.emailjs.sendForm(
        "service_iutw2en",
        "template_bwjmmwu",
        formulario
      )
      .then(() => {
        alert("Seu e-mail foi enviado. Em breve entrarei em contato!");
        formulario.reset();
      })
      .catch((erro) => {
        console.error("Erro ao enviar o e-mail:", erro);
        alert("Erro ao enviar. Por favor, tente novamente.");
      });
    }
  }
}
</script>
