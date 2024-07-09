<template>
  <nav>
      <ul>
        <li>
          <a class="logo" href="#" rel="noopener noreferrer">
            <img
              src="../../public/assets/logo.svg"
              alt="Logo funilaria"
            />
          </a>
        </li>
      </ul>
      <ul>
        <li>
          <a href="#" rel="noopener noreferrer">Serviços</a>
        </li>
        <li>
          <a href="#" rel="noopener noreferrer">Resultados</a>
        </li>
        <li class="d-flex align-items-baseline">
          <b-icon icon="pin-map" class="me-2"></b-icon>
          <a href="#" rel="noopener noreferrer">Localização</a>
        </li>
        <li>
          <a class="btn" href="#" rel="noopener noreferrer">
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