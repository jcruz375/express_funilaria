<template>
  <section
    id="serviços"
    class="d-flex flex-column justify-content-center align-items-center mb-5"
  >
    <h2>Serviços</h2>
    <b-row class="mt-5 px-5">
      <template v-for="(servico, index) in servicos">
        <b-col
          :key="index"
          cols="12"
          md="5"
          class="d-flex flex-column align-items-center justify-content-center card"
        >
          <span>{{ servico.name }}</span>
          <img
            :src="getImagePath(servico.image)"
            :alt="servico.description"
            :title="servico.description"
          />
          <p class="text-center mt-2 w-75">{{ servico.description }}</p>
        </b-col>
      </template>
    </b-row>
    <a href="https://api.whatsapp.com/send?phone=5511994718878" target="_blank" rel="noopener noreferrer" class="btn-wpp mt-5">
      <i class="fab fa-whatsapp"></i>
      Solicitar orçamento
    </a>
  </section>
</template>

<script>
export default {
  data() {
    return {
      servicos: [
        {
          name: "Funilaria e pintura",
          image: "carro-1",
          description: "Realizamos serviços completos de funilaria e pintura para restaurar a estética e a integridade do seu veículo, utilizando materiais de alta qualidade e técnicas avançadas.",
        },
        {
          name: "Martelinho de ouro",
          image: "martelinho",
          description: "Oferecemos o serviço de martelinho de ouro para corrigir amassados sem a necessidade de repintura, preservando a pintura original do veículo.",
        },
        {
          name: "Polimento especializado",
          image: "polimento",
          description: "Nosso polimento especializado remove riscos, manchas e imperfeições da pintura, devolvendo o brilho e a beleza original do seu carro.",
        },
        {
          name: "Pequenos reparos",
          image: "pequenos",
          description: "Efetuamos pequenos reparos na lataria e na pintura do seu veículo, garantindo uma solução rápida e eficiente para pequenos danos.",
        },
        {
          name: "Restauracao de para choques",
          image: "brilho",
          description: "Especialistas em restaurar para-choques e retrovisores danificados, trazendo de volta a aparência e a funcionalidade originais.",
        },
      ],
    };
  },

  methods: {
    getImagePath(imageName) {
      return `/assets/services/${imageName}.jpg`;
    },
  },
};
</script>

<style lang="scss" scoped>
@import "../sass/global.scss";
img {
  width: 341px;
  height: 226px;
  border-radius: 8px;
}

.row {
  display: flex;
  flex-wrap: wrap;
  justify-content: center;
  gap: 1rem;
}

.card {
  background: #000;
  border-radius: 1rem;
  padding: 1rem;
  gap: 1rem;
  box-shadow: rgba(0, 0, 0, 0.3) 0px 19px 38px, rgba(0, 0, 0, 0.22) 0px 15px 12px;
  cursor: pointer;
  span {
    font-size: 2rem;
    text-align: center;
    font-weight: 700;
    color: $orange;
    margin-bottom: 8px;
  }
  p {
    color: $orange;
  }

  transition: 0.3s;
  &:hover {
    transform: scale(1.03);
    box-shadow: none;
  }
}
</style>