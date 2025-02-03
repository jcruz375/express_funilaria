<template>
  <footer>
    <b-container>
      <section
        class="d-flex flex-column justify-content-center align-items-center mb-5"
      >
        <h3>Entre em contato!</h3>
        <a
          href="https://api.whatsapp.com/send?phone=5511994718878"
          target="_blank"
          rel="noopener noreferrer"
          class="btn-wpp mt-3"
        >
          <i class="fab fa-whatsapp"></i>
          (11) 99471-8878
        </a>
        <!-- <a
          class="email_link mt-3"
          href="mailto:contato@expressfunilaria.com"
          target="_blank"
          rel="noopener noreferrer"
        >
          <i class="fa-regular fa-envelope"></i>
          contato@expressfunilaria.com
        </a> -->
        <article class="text-center mt-3">
          Segunda a sexta das 8:00 ás 18:00
        </article>
        <article class="text-center mt-3">
          Avenida Getúlio Vargas 1778 baeta Neves São Bernardo do Campo
        </article>
      </section>
    </b-container>
  </footer>
</template>

<script>
/* eslint-disable */
export default {};
</script>

<style lang="scss" scoped>
@import "../sass/global.scss";
footer {
  padding: 2rem;
  background: #e06f30;
  min-height: 200px;
  color: #fff;

  .email_link {
    color: #fff;
    text-decoration: none;
  }

  article {
    width: 500px;
    @media (max-width: 768px) {
      width: 400px;
      margin-top: 1rem;
      &:first-child {
        border-right: none;
      }
      border: none;
    }
  }
}
</style>  