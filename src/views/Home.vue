<script>
import NavBar from '../components/NavBar.vue';
import AcadFooter from '../components/AcadFooter.vue';
import BtnScroll from '../components/BtnScroll.vue';
export default {
  components: {
    NavBar, AcadFooter, BtnScroll
  },
  data() {
    return { rerender: 0 }
  },
  methods: {
    forceRerender() {
      this.rerender++
    }
  },
  mounted() {
    this.forceRerender()
  }
}

</script>

<template>
  <NavBar :key="rerender"></NavBar>
  <section>

    <div id="carousel" class="carousel slide">
      <div class="carousel-inner">
        <div class="carousel-item active">
          <img src="../../images/abs-g468a22f11_1280.jpg" class="d-block w-100" alt="...">
          <div class="carousel-caption d-md-block text-center">
            <h5>Quem Somos?</h5>
            <p>Uma Acadeia Voltada Para Aumentar seu Desempenho! </p>
          </div>
        </div>
        <div class="carousel-item">
          <img src="../../images/exercise-weights-iron-dumbbell-with-extra-plates.jpg" class="d-block w-100" alt="...">
          <div class="carousel-caption d-md-block text-center">
            <h5>Onde estamos?</h5>
            <p>Procure por nossa academia mais proxima de sua residencia! </p>
          </div>
        </div>
        <div class="carousel-item">
          <img src="../../images/training-ge79437eb8_1280.jpg" class="d-block w-100" alt="...">
          <div class="carousel-caption d-md-block text-center">
            <h5>Duvidas no treino?</h5>
            <p>Entre em contato com uns de nossos personais e tire suas duvidas!</p>
          </div>

        </div>
      </div>
      <button class="carousel-control-prev" type="button" data-bs-target="#carousel" data-bs-slide="prev">
        <span class="carousel-control-prev-icon" aria-hidden="true"></span>
        <span class="visually-hidden">Previous</span>
      </button>
      <button class="carousel-control-next" type="button" data-bs-target="#carousel" data-bs-slide="next">
        <span class="carousel-control-next-icon" aria-hidden="true"></span>
        <span class="visually-hidden">Next</span>
      </button>
    </div>
  </section>
  <section id="atividades">
    <ul id="nossas_atividades">
      <li class="atividade">
        <h2 class="titulo_atividade">Muscula????o</h2>
        <p class="descricao_atividade">
          Aqui voc?? encontra os melhores equipamentos de muscula????o para ficar
          com o f??sico pronto para o ver??o.
        </p>
        <p class="preco_atividade">R$ 149,90</p>
      </li>
      <li class="atividade">
        <h2 class="titulo_atividade">Boxe</h2>
        <p class="descricao_atividade">
          Aulas de boxe com os melhores instrutores da cidade
          para voc?? aprender a arte dos ringues e se manter na melhor forma.
        </p>
        <p class="preco_atividade">R$ 199,99</p>
      </li>
      <li class="atividade">
        <h2 class="titulo_atividade">Jiu-jitsu</h2>
        <p class="descricao_atividade">
          Aprenda essa luta que consagrou diversos brasileiros pelo mundo.
          Temos os melhores instrutores aqui.
        </p>
        <p class="preco_atividade">R$ 199,99</p>
      </li>
      <li class="atividade">
        <h2 class="titulo_atividade">Nata????o</h2>
        <p class="descricao_atividade">
          Venha fazer esse exerc??cio que al??m de ser um dos melhores para a sa??de
          e condicionamento f??sico, ainda ?? refrescante. (Temos piscina aquecida para o inverno)
        </p>
        <p class="preco_atividade">R$ 169,99</p>
      </li>
      <li class="atividade">
        <h2 class="titulo_atividade">Bike Indoor</h2>
        <p class="descricao_atividade">
          ?? um exerc??cio aer??bico que mistura elementos de diferentes ritmos, como salsa, samba, reggaet??n e at?? mesmo
          hip-hop, tornando-se uma dan??a divertida, mas que queima muitas calorias!
        </p>
        <p class="preco_atividade">R$ 119,99</p>
      </li>
      <li class="atividade">
        <h2 class="titulo_atividade">Jump</h2>
        <p class="descricao_atividade">
          Aula pr??-coreografada moderada a intensa com objetivo de melhorar o f??lego, a
          resist??ncia muscular e a coordena????o motora utilizando um mini-trampolim.
        </p>
        <p class="preco_atividade">R$ 119,99</p>
      </li>
    </ul>
  </section>
  <section id="quem-somos">
    <div class="academia">
      <h2>Queremos falar um pouco sobre n??s</h2>
      <p>
        Estamos localizados na Av taltaltal n?? 777
        Chapa Quente - RJ Brasil.
        Estamos no mercado h?? mais de 10 anos, tendo todo carinho e aten????o com nossos alunos, trazendo para eles a auto
        estima para poder cuidar da sua sa??de. Temos diversas modalidades para voc?? se desafiar.
      </p>
      <P>
        Temos tamb??m professores muito capacitados para auxiliar nossos alunos, em busca de um ??timo
        resultado.
      </P>
    </div>

    <div id="professores" class="nomes">
      <p>
        Esses s??o nossos professores
      </p>

      <div>
        <span class="boxe">
          <img src="../../images/boxe.jpg" alt="boxe" width="250" height="250" class="boxe">
          <p>Arthur Maliano - 34 anos, profissional h?? mais de 10 anos na ??rea do boxe. Ele est?? disposto a ajudar os
            alunos
            para emagrece e se defender.</p>
        </span>
        <span class="bikeindoor">
          <img src="../../images/baker-indoor.jpg" alt="bike indoor" width="250" class="bike indoor">
          <p>Thiago Gomes - 30 anos, profissional durante 7 anos, j?? ajudou v??rias pessoas a atingir sua melhor forma e
            ter
            uma vida
            saud??vel.</p>
        </span>

        <span class="jiujitsu">
          <img src="../../images/jiujitsu.jpg" alt="jiujitsu" width="250" class="jiujitsu">
          <p>Carlos Alberto - 44 anos mestre de jiujitsu, tem diversas medalhas de compeonato e est?? disposto a formar
            futuros campe??es de jiujitsu.</p>
        </span>
        <span class="musculacao">
          <img src="../../images/muscula????o.jpg" alt="muscula????o" width="250" class="muscula????o">
          <p>Rafael Dias - 30 anos, personal com grande conhecimento na ??rea para ajudar as pessoas que est??o tendo
            difilcudades em atingir sua melhor forma.</p>
        </span>

        <span class="jump">
          <img src="../../images/jump.jpg" alt="jump" width="250" class=" jump">
          <p>Leticia Ribeiro - 30 anos, professora muito procurada nesta ??rea, por conta de seu trabalho bem
            delicado para que n??o venha prejudicar os alunos que tem problema de sa??de mas que queira fazer o jump.</p>
        </span>
        <span class="natacao">
          <img src="../../images/nata????o.jpg" alt="nata????o" width="255" class="nata????o">
          <p>Ricardo Gomes- 25 anos, ele tem um ??timo trabalho de nata????o ao povo de terceira idade, crian??as, tendo a
            responsabilidade de dar o m??ximo suporte que o aluno esteja precisando.</p>
        </span>
      </div>

    </div>

  </section>
  <AcadFooter></AcadFooter>
  <BtnScroll></BtnScroll>
</template>

<style scoped>
html {
  scroll-behavior: smooth;
}

.carousel-inner {
  max-height: 100vh;
  position: relative;
}

.carousel-caption h5 {
  font-size: 7vw;
  /* margin-bottom: 15px; */
  color: var(--secondary);
}

.carousel-caption p {
  font-size: 3vw;
  font-weight: 300;
  margin-bottom: 35%;
  color: var(--white);
}


#atividades {
  min-height: 100vh;
  background-color: var(--primary);
  align-content: center;
  color: var(--white);
}

#atividades ul {
  padding: 2rem;
  display: grid;
  grid-template-columns: repeat(3, 1fr);
  gap: 2rem;
  margin: 0;
}

#atividades .atividade {
  display: flex;
  flex-direction: column;
  justify-content: space-evenly;
  padding: 1rem;
  min-height: 400px;
  line-height: 2;
  list-style: none;
  place-self: center;
  border-radius: .5rem;
  border: solid 2px #FFA41C;
  text-align: center;
}

.atividade .preco_atividade {
  font-size: 1.5rem;
}

#professores>p {
  margin-bottom: 2rem;
  font-size: 26px;
  font-weight: 600;
}

#professores img {
  height: 150px;
  width: 150px;
  clip-path: circle();
}

.academia {
  background-color: #202020;
  color: white;
  padding: 50px;
}

.academia h2 {
  font-size: 2rem;
}

.nomes {
  background-color: var(--primary);
  color: white;
  padding: 50px;
}

.boxe,
.bikeindoor,
.jiujitsu,
.musculacao,
.jump,
.natacao {
  display: flex;
  align-items: center;
  gap: 1.5rem;
  margin-bottom: 1.5rem;
}


@media screen and (max-width: 1000px) {
  #atividades ul {
    grid-template-columns: repeat(2, 1fr);
  }

  .carousel-caption p {
    margin-bottom: 30%;
  }

}

@media screen and (max-width: 768px) {
  #atividades ul {
    grid-template-columns: 1fr;
  }

  #atividades li {
    max-width: 400px;
  }

  .carousel-caption p {
    margin-bottom: 25%;
  }

  #professores>p {
    text-align: center;
  }

  .boxe,
  .bikeindoor,
  .jiujitsu,
  .musculacao,
  .jump,
  .natacao {
    flex-direction: column;
    text-align: justify;
  }

  .boxe p,
  .bikeindoor p,
  .jiujitsu p,
  .musculacao p,
  .jump p,
  .natacao p {
    padding: 1.5rem;
  }
}
</style>
