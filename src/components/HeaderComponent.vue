<template>
  <nav>
      <ul>
        <li>
          <a class="logo" href="#" target="blank" rel="noopener noreferrer">
            <img
              src="../../public/assets/logo.svg"
              alt="Logo funilaria"
            />
          </a>
        </li>
      </ul>
      <ul>
        <li>
          <a href="#" target="blank" rel="noopener noreferrer">Serviços</a>
        </li>
        <li>
          <a href="#" target="blank" rel="noopener noreferrer">Resultados</a>
        </li>
        <li>
          <a class="btn" href="#" target="blank" rel="noopener noreferrer">
            <!-- <FaWhatsapp /> -->
            <i class="fab fa-whatsapp"></i>
            Entre em contato
          </a>
        </li>
      </ul>
    </nav>
</template>

<script>
export default {

}
</script>

<style lang="scss" scoped>
  @import '../sass/global.scss';
  @import '../sass/components/layout/header.scss';
</style>