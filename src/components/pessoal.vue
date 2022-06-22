<template>
  <section id="sobre-mim" class="bg-fantasma">
    <div class="container animate__animated animate__fadeInUp">
      <h2 class="h2">
        Sobre mim
      </h2>
      <hr class="tt-bar">
      <div class="row mt-4">
        <div class="col-8 ms-auto me-auto">
          <div class="row">
            <div class="col-sm-3 d-flex flex-column">
              <strong>11 anos</strong>
              <span>Experiência</span>
            </div>
            <div class="col-sm-3 d-flex flex-column">
              <strong>32</strong>
              <span>Idade</span>
            </div>
            <div class="col-sm-3 d-flex flex-column">
              <strong>Vitória - ES</strong>
              <span>Residencia</span>
            </div>
            <div class="col-sm-3 d-flex flex-column">
              <strong>+100</strong>
              <span>Projetos</span>
            </div>
          </div>
        </div>
      </div>
      <div class="row mt-4">
        <div class="col-sm-8 ms-auto me-auto animate__animated animate__fadeInUp">
          <p class="text-justfy">
            Sou profissional da área de tecnologia desde 2012, minha carreira começou como uma boa parte dos profissionais da área, por entusiasmo e curiosidade, em 2007 eu me lembro de ter feito meu primeiro inspecionar elemento na página do Google e mudei a cor de fundo. Belo hacker eu era kkk.
          </p>
          <p class="text-justfy animate__animated animate__fadeInUp">
            Iniciei meu aprendizado com cursos básicos de computação em 2008 fiz meu primeiro curso de HTML, mas só comecei a atuar como DEV em 2012 quando cheguei em Vitória no Espírito Sando, entrei para uma fábrica de software que atendia diversas agências e clientes no estado, onde tive a oportunidade trabalhar para grandes marcas e pude aprender e ampliar meu conhecimento no frontend, backend e gestão de projetos.
          </p>
          <p class="text-justfy animate__animated animate__fadeInUp">
            Atualmente atuo como desenvolvedor autônomo desde 2020 prestando serviço para várias empresas, minha atuação é focada em criação de sistemas web, gosto de trabalhar com Javascript+VUE.JS e com PHP+Laravel, porém os principais projetos que atuo hoje em dia, são com C# .net standard.
          </p>
          <div  class="text-center animate__animated animate__fadeInUp">
            <h4 class="h3">
              Contato
            </h4>
            <br>
          </div>
          <div class="row">
            <div class="col-6">
              <a href="tel:+5527981539221" class="text-white text-bold text-decoration-none">
                <i class="fas fa-mobile-alt text-white text-bold fs-3"></i><br> +55 27 9 8153-9221
              </a>
            </div>
            <div class="col-6">
              <a href="mailto:deivid@dgmattos.com.br" class="text-white text-bold text-decoration-none">
                <i class="fas fa-envelope text-white text-bold fs-3"></i><br> deivid@dgmattos.com.br
              </a>
            </div>
          </div>
        </div>
      </div>
      <h2 class="h2 mt-5">
        Skills
      </h2>
      <hr class="tt-bar">
      <h3 class="h3 mt-5">
        <i class="fas fa-grin-hearts"></i> Stack favorita <i class="fas fa-grin-hearts"></i>
      </h3>
      <div class="row">
        <div class="col-sm-12">
          <img class="logo-circle" src="/src/assets/logos-stack/logo-vue.png" alt="VUE JS Na Veia" title="VUE JS">
          <img class="logo-circle" src="/src/assets/logos-stack/logo-laravel.png" alt="Laravel" title="Laravel">
          <img class="logo-circle" src="/src/assets/logos-stack/logo-sqlserver.png" alt="SQLSERVER" title="SQLSERVER">
        </div>
      </div>
      <h3 class="h3 mt-5">
        Outras tecnologias
      </h3>
      <div class="row">
        <div class="col-sm-12">
          <img class="logo-circle" src="/src/assets/logos-stack/logo-csharp.png" alt="C#" title="C#">
          <img class="logo-circle" src="/src/assets/logos-stack/logo-html.png" alt="HTML5" title="HTML5">
          <img class="logo-circle" src="/src/assets/logos-stack/logo-css.png" alt="CSS/SCSS/SASS" title="CSS/SCSS/SASS">
          <img class="logo-circle" src="/src/assets/logos-stack/logo-javascript.png" alt="Javascript" title="Javascript">
          <img class="logo-circle" src="/src/assets/logos-stack/logo-php.png" alt="PHP" title="PHP">
          <img class="logo-circle" src="/src/assets/logos-stack/logo-mysql.png" alt="Javascript" title="Javascript">
          <img class="logo-circle" src="/src/assets/logos-stack/logo-arduino.png" alt="Arduino" title="Arduino">
          <img class="logo-circle" src="/src/assets/logos-stack/logo-flutter.png" alt="Flutter" title="Flutter">
        </div>
      </div>
      <h3 class="h3 mt-5">
        Experiência Profissional
      </h3>
      <hr class="tt-bar">
      <div class="row">
        <div class="col-sm-10 ms-auto me-auto">
          <table class="table table-striped">
            <tr class="período">
              <th class="text-white">Empresa</th>
              <th class="text-white">Cargo</th>
              <th class="text-white">Período</th>
              <th class="text-white">Formato</th>
            </tr>
            <tr>
              <td>Teknow tecnologia</td>
              <td>Full-stack</td>
              <td>2011 até 2013</td>
              <td>CLT</td>
            </tr>
            <tr>
              <td>Betha Espaço imóveis</td>
              <td>Full-stack</td>
              <td>2013 até 2020</td>
              <td>CLT</td>
            </tr>
            <tr>
              <td>Betha Espaço imóveis</td>
              <td>Full-stack</td>
              <td>2020 até o momento</td>
              <td>PJ</td>
            </tr>
            <tr>
              <td>Causei o bem</td>
              <td>Full-stack</td>
              <td>2020 até o momento</td>
              <td>PJ</td>
            </tr>
          </table>
        </div>
      </div>
    </div>
  </section>
</template>

<script>
export default {
  name: "pessoal"
}
</script>

<style scoped>
.logo-circle {
  max-width: 120px;
}
</style>