<template>
  <div class="banner">
    <img
      src="../assets/magnetisme.png"
      alt="magnetisme-image"
      class="banner-img"
    />
    <h2 class="banner-title">Soins energetiques-Magnetisme</h2>
  </div>
  <div class="description-card">
    <h3 class="title">Massage Metamorphique</h3>
    <div class="borderTop"></div>
    <div class="story">
      <h4 class="chapter">Un peu d'histoire</h4>
      <div class="card-items">
        De nombreux hiéroglyphes, illustrations et papyrus montrent que l'on
        magnétisait déjà les hommes comme les plantes dans l'Egypte Antique, du
        temps des Pharaons.<br />
        Les recherches archéologiques menées dans les ruines de Thèbes ont mis
        au jour des représentations des prêtres d'Isis et d'Osiris employant
        l'imposition des mains pour apaiser les maux des vivants ou pour aider
        les défunts à passer dans l'au-delà.<br />
        Un papyrus découvert parmi les vestiges de Thèbes contient cette formule
        : pose ta main sur la douleur et ordonne lui de s'en aller. C'est une
        alusion claire à l'imposition des mains servant à faire passer le fluide
        magnétique d'un individu à l'autre. <br />Au XI ème siècle, Alexandre de
        Tralles (527 -565) médecin Grec, disait que l'imposition des mains
        permettait le transfert d'un fluide mystérieux et énergétique qui
        provoque l'élimination des principes morbides, calme, régularise et
        tonifie le corps.<br />
        Au XV ème siècle, Pietro Pompanazzi, philisophe et médecin, a écrit dans
        ses Admirables Effets de la Nature : "... Il y a des hommes qui
        possèdent des propriétés salutaires et puissantes. Ces propriétés
        s'exalent par la force de l'imagination et du désir et produisent sur
        les corps qui reçoivent des effets remarquables. L'âme exerce son empire
        par la transmission de certaines vapeurs subtiles."
        <h4 class="chapter">Qu'est ce que le magnétisme</h4>
        Le Magnétisme est un transfert d'énergie vitale.<br />
        Cette énergie vitale est le courant qui anime la vie. <br />Le
        Magnétisme soulage, aide, permet d'améliorer, de soutenir, la guérison
        du corps émotionnel, physique et énergétique.<br />
        Il permet de travailler sur tous les corps.<br />
        L'énrergie ne fait pas de différence entre les problèmes physiques et
        émotionnels. Elle va où elle est nécessaire et répond aux besoins de la
        personne.
        <h4 class="chapter">Le magnetisme peut vous aider à</h4>
        - Apaiser votre mental<br />
        - Vous libérer du stress<br />
        - De certaines peurs ou angoisses.<br />
        Il agit sur les causes émotionnelles qui sont à l'origine de certains
        symptômes et douleurs car toutes émotions bloquées entrainent un blocage
        énergétique. Les problèmes émotionnels non résolus peuvent bloquer les
        vibrations de guérison, entraînant le retour de la maladie. Corps et
        Esprit sont bel et bien liés.<br />
        L'énergie n'est ceprendant pas là pour guérir les problèmes émotionnels
        de la personne mais plutôt pour l'aider à se sentir plus équilibrée,
        ancrée et centrée, de façon à ce qu'elle puisse travailler plus
        efficacement sur ses émotions.<br /><br />
        Chaque personne possède en elle toutes les ressources nécessaires pour
        manifester l'auto-guerison. Par mon travail je vais libérer les énérgies
        troubles et ramener de l'énergie saine pour favoriser les mécanismes de
        celle-ci. J'agis simplement en catalyseur qui vous permet de vous guérir
        vous-mêmes.
        <h4 class="chapter">Déroulement d'une séance</h4>
        La séance commence par un temps d'échange afin de cibler votre
        demande.<br />
        Les soins s effectuent par imposition des mains.<br />
        J'agis en suivant mes ressentis, mon intuition et mon coeur.<br />
        Mes mains agissent en capteurs, elles scannent et détectent les zones où
        les vibrations sont dysharmonieuses dans le champ énergétique, les zones
        du corps en tension et les charges émotionnelles. Ce sont de véritables
        guides.<br />
        Si la demande n'est pas ciblée, je vais scanner l'ensemble de votre
        corps. La séance consiste à aller libérer les énergies cristalisées,
        recharger les zones en faiblesse et consolider le corps énergétique.<br />
        Le retour après séance est important car il permet de faire le point sur
        les ressentis et le vécu pendant le soin de la personne.
        <div class="card-details">
          Les soins s'adressent à toutes personnes en souffrance adulte ou
          enfant. Ils peuvent être effectués en présence ou à distance.<br />
          La durée du massage est de 1 h.
        </div>
      </div>
    </div>
  </div>
</template>

<script>
export default {
  name: "Magnetisme",
  data() {
    return {
      seeMore: null,
    };
  },
  methods: {
    handleClick(event) {
      if (event.target.textContent === "Voir Détails") {
        this.seeMore = true;
        event.target.textContent = "Réduire Détails";
      } else {
        this.seeMore = !true;
        event.target.textContent = "Voir Détails";
      }
      return;
    },
  },
};
</script>

<style scoped>
.banner {
  display: flex;
  position: relative;
  margin: 8rem 0rem 1rem 0rem;
  min-height: 6.5rem;
  background-color: #643f8a;
  box-shadow: rgba(0, 0, 0, 0.315) 0px 10px 20px,
    rgba(0, 0, 0, 0.363) 0px 6px 6px;
}

.banner-title {
  align-self: center;
  margin: auto;
  font-size: 2rem;
}

.banner-img {
  position: absolute;
  left: 350px;
  height: 85px;
  width: 125px;
  margin: 0.5rem;
}

.description-card {
  background-color: #653f8ad5;
  box-shadow: rgba(0, 0, 0, 0.315) 0px 10px 20px,
    rgba(0, 0, 0, 0.363) 0px 6px 6px;
  padding: 1rem;
  margin-bottom: 1rem;
}

.more-details {
  margin-top: 1.5rem;
}

.title {
  text-align: center;
  text-transform: uppercase;
  width: 300px;
  margin: auto;
  background: rgb(44, 21, 76);
  background: linear-gradient(
    90deg,
    rgba(44, 21, 76, 1) 65%,
    rgba(113, 73, 151, 1) 100%
  );
  box-shadow: rgba(255, 255, 255, 0.35) 0px 5px 15px;
}

.chapter {
  text-align: center;
}

.expand-link {
  margin-left: 1rem;
  text-decoration: underline;
  text-underline-offset: 3px;
}

.card-details {
  text-align: center;
  margin-top: 3rem;
}

.expand-link:hover {
  cursor: pointer;
  font-size: 1.2rem;
  color: rgb(61, 18, 58);
  transition: 0.5s ease all;
}

.story {
  position: relative;
  margin: 0rem 3rem 0rem 3rem;
  padding: 2rem 3rem 2rem 3rem;
  border-left: solid;
}

.story::before {
  content: "";
  display: block;
  position: absolute;
  top: 0;
  width: 10%;
  left: 0;
  border-top: 2px solid white;
}

.story::after {
  content: "";
  display: block;
  position: absolute;
  bottom: 0;
  width: 10%;
  left: 0;
  border-top: 2px solid white;
}

.chapter {
  font-size: 1.3rem;
  font-style: italic;
  text-decoration: underline;
}
</style>
