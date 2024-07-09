<template>
  <b-navbar toggleable="lg" type="dark" variant="primary" class="custom-navbar">
    <b-navbar-brand href="#">
      <img
        src="../../public/assets/logo.svg"
        alt="Logo funilaria"
        class="logo"
      />
    </b-navbar-brand>

    <b-navbar-toggle target="nav-collapse"></b-navbar-toggle>

    <b-collapse id="nav-collapse" is-nav class="justify-content-end">
      <b-navbar-nav class="ml-auto">
        <b-nav-item href="#">Serviços</b-nav-item>
        <b-nav-item href="#">Resultados</b-nav-item>
        <b-nav-item href="#">
          <b-icon icon="geo-alt" class="me-2"></b-icon>
          Localização
        </b-nav-item>
        <b-nav-item href="#" class="btn-wpp">
          <i class="fab fa-whatsapp"></i>
          Entre em contato
        </b-nav-item>
      </b-navbar-nav>
    </b-collapse>
  </b-navbar>
</template>

<script>
export default {};
</script>

<style lang="scss" scoped>
@import '../sass/variables.scss';

.custom-navbar {
  display: flex;
  justify-content: center;
  align-items: center;
  padding: 1.5rem;
  background-color: #000 !important;
  width: 100%;
  font-weight: 700;

  .navbar-nav {
    list-style: none;
    margin-bottom: 0;
    display: flex;
    align-items: center;

    .nav-item {
      .nav-link {
        color: $orange;
        text-decoration: none;
        position: relative;

        &::after {
          content: "";
          display: block;
          width: 0;
          height: 4px;
          border-radius: 4px;
          background: $orange;
          transition: width 0.3s;
          position: absolute;
          bottom: -5px;
          left: 0;
        }

        &:hover::after {
          width: 100%;
        }

        &.logo::after {
          display: none;
        }
      }
    }
  }

  .btn-wpp {
    a {
      color: #FFFFFF !important;
      &:hover {
        &::after {
          display: none !important;
      }
    }
    }
  }

  .navbar-nav:last-child {
    gap: 3rem;

    .nav-item {
      color: $orange;
      font-size: 1.8rem;
    }
  }
} 

@media (max-width: 768px) {
  .custom-navbar {
    justify-content: space-between;
  }
  .navbar-nav {
    gap: 0.5rem !important;
    align-items: flex-start !important;
  }
}
</style>
