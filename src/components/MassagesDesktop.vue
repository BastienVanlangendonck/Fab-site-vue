<template>
  <div class="banner">
    <img
      src="../assets/massages.png"
      alt="magnetisme-image"
      class="banner-img"
    />
    <h2 class="banner-title">Massages</h2>
  </div>
  <div class="description-card">
    <h3 class="title">Massage Metamorphique</h3>
    <div class="borderTop"></div>
    <div class="story">
      <h4 class="chapter">A qui s'adresse le massage métamorphique ?</h4>
      Cette technique est bénéfique pour :<br /><br />
      - Toutes les personnes intéressées par un développement personnel.<br />
      - Les personnes en situation de handicap physiques et psychiques.<br />
      - A tous ceux ou celles qui veulent faire la paix avec leur naissance.<br />
      - Aux femmes enceintes, pour atténuer l'anxiété et les angoisses qui
      accompagnent souvent la grossesse.<br />
      - Aux enfants de tous âges.<br />
      - Les naissances difficiles qui ont pu occasionner certains traumatismes
      physiques ou psychologiques.<br />
      - Les problèmes de communication et de langage, souvent reliés à la
      conception.
      <h4 class="chapter">Un peu d'histoire</h4>
      <div class="card-items">
        Le massage Métamorphique a été crée par Robert St John, Naturopathe et
        réflexologue. Il a voyagé dans de nombreux pays du monde entier où il
        pratiquait et enseignait la métamorphose. Son but était de trouver un
        moyen d'aider les gens à s'aider eux-mêmes. Il résolut de trouver une
        approche qui fonctionnerait à un niveau absolument fondamental et était
        conscient que la condition physique était une manifestation de
        l'attitude mentale. Le changement d'attitude devaît être fait par la
        personne elle-même et non pas par l'acceptation de la volonté d'un
        autre. Dans les années 50, Robert St John a observé que le travail sur
        la zone réflexe de la colonne vertébrale au niveau des pieds, des mains
        et de la tête, au-delà d'une influence sur le physique, avait
        principalement une incidence sur le psychisme. Les bases complètes de
        son travail sont issues de sa pratique en naturopathie, en réflexologie
        et du travail de rééducation qu'il a effectué avec un enfant Autiste.
        Robert St John avait une connaissance profonde de la période prénatale
        et cette technique "Métamorphique" permet de revenir à la source de nos
        blocages et d'en nettoyer directement les mémoires tout en libérant
        notre lignée. Dans la nature un gland devient un chêne, une chenille se
        métamorphe en papillon. En nous aussi un potentiel d'évolution existe,
        qui augmente notre champ d'action et nous permet de devenir bien plus
        que ce que nous sommes.
        <h4 class="chapter">Bienfaits du massage métamorphique</h4>
        Des mémoires inconscientes, acquises lors de la gestation, forment une
        partie de nos caractéristiques et imprègnent notre vie consciente. Le
        but est donc de solliciter des zones réflexes, afin de faire émerger et
        libérer des souffrances qui nuisent à notre épanouissement, et
        parrallèlement de réveiller notre pouvoir intérieur de guérison. L'homme
        a, au niveau instinctif, le pouvoi de se guérir lui-même. Nous devons
        rester conscient qu'en nous réside une grande puissance de guérison. Par
        le toûcher en Métamorphose, il est possible de libérer le potentiel de
        la structure de cette période de conception et ainsi entamer un
        processus de transformation pour aller de qui nous sommes à qui nous
        pouvons être.
        <h4 class="chapter">Ce massage agira afin d'aider à</h4>
        - Dépasser une situation, <br />
        - Gagner en confiance,<br />
        - Changer de mode de vie,<br />
        - S'éveiller à son potentiel,<br />
        - Lâcher prise,<br />
        - Prendre conscience de ses blocages,<br />
        - Développer une meilleure estime de soi,<br />
        - Voir les choses sous un autre angle,<br />
        - Eliminer toutes mémoires du passé *
        <a class="expand-link" @click="handleClick">Voir Détails</a>
        <div v-show="seeMore" class="more-details">
          Mémoires cellulaires (expériences vécues, patrimoine génétique de
          notre karma de mémoires collectives, transgéniques - croyances et
          conditionnements qui se mémorisent dans nos cellules).<br /><br />
          * Mémoires collectives (représentation d'un groupe - souvenir ou
          ensemble de souvenirs conscients ou non d'une expérience vécue par une
          collectivité vivante).<br />
          *Mémoires transgéniques (transmission familiale, intergénérationnelles
          et transgénérationnelles).<br />
          * Mémoires karmiques (répercussion de nos actes dans nos vies passés +
          pactes passés dans des vies antérieurs).<br />
          *Mémoires liées à la conception (contexte dans lequel nous sommes
          conçus).<br />
          * Mémoires liées à la période de gestation (évènement que vit la mère
          pendant 9 mois).<br />
          * Mémoires liées à la naissance (condition de l'accouchement).
        </div>
        <div class="card-details">
          Les zones massées sont les pieds, les mains, et la tête.<br />
          La durée du massage est de 1 h.
        </div>
      </div>
    </div>
  </div>
</template>

<script>
export default {
  name: "MassagesDesktop",
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
  width: 175px;
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
