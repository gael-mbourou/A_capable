<template>
  <div class="accordion" role="tablist">
    <b-card no-body class="mb-1">
      <b-card-header header-tag="header" class="p-1" role="tab">
        <b-button block v-b-toggle.accordion-1 variant="info">Hygiène et confort</b-button>
      </b-card-header>
      <b-collapse id="accordion-1" visible accordion="my-accordion" role="tabpanel">
        <b-card-body>
          <b-card-text>{{ text1 }}</b-card-text>
        </b-card-body>
      </b-collapse>
    </b-card>

    <b-card no-body class="mb-1">
      <b-card-header header-tag="header" class="p-1" role="tab">
        <b-button block v-b-toggle.accordion-2 variant="info">Nettoyage et entretien du logement</b-button>
      </b-card-header>
      <b-collapse id="accordion-2" accordion="my-accordion" role="tabpanel">
        <b-card-body>
          <b-card-text>{{ text2 }}</b-card-text>
        </b-card-body>
      </b-collapse>
    </b-card>

    <b-card no-body class="mb-1">
      <b-card-header header-tag="header" class="p-1" role="tab">
        <b-button block v-b-toggle.accordion-3 variant="info">Préparation des repas</b-button>
      </b-card-header>
      <b-collapse id="accordion-3" accordion="my-accordion" role="tabpanel">
        <b-card-body>
          <b-card-text>{{ text3 }}</b-card-text>
        </b-card-body>
      </b-collapse>
    </b-card>

    <b-card no-body class="mb-1">
      <b-card-header header-tag="header" class="p-1" role="tab">
        <b-button block v-b-toggle.accordion-4 variant="info">Aide au levé et au couché</b-button>
      </b-card-header>
      <b-collapse id="accordion-4" accordion="my-accordion" role="tabpanel">
        <b-card-body>
          <b-card-text>{{ text4 }}</b-card-text>
        </b-card-body>
      </b-collapse>
    </b-card>

    <b-card no-body class="mb-1">
      <b-card-header header-tag="header" class="p-1" role="tab">
        <b-button block v-b-toggle.accordion-5 variant="info">Entretien du linge</b-button>
      </b-card-header>
      <b-collapse id="accordion-5" accordion="my-accordion" role="tabpanel">
        <b-card-body>
          <b-card-text>{{ text5 }}</b-card-text>
        </b-card-body>
      </b-collapse>
    </b-card>
  </div>
</template>

<script>
  export default {
      name:'Accordeon',
    data() {
      return {
        text1: `
          • Nettoyage régulier
          • Entretien des sanitaires et matériels selon les règles d’hygiène domestique
        `,
        text2: `
        Rangement des pièces habitées en respectant les souhaits de la personne
        Dépoussiérage et cirage des meubles
        Balayage, passage de l’aspirateur, lavage et lessivage des sols
        Nettoyage des vitres et des encadrements
        Entretien des plantes intérieures
        Nettoyage des abords de la maison
        Nettoyage du matériel de cuisson après usage (four, plaques…)
        Vérification du bon état de fonctionnement
        `,
        text3: `
          • Préparation de repas simples et équilibrés
            • Préparation de repas de régimes conformément à la prescription médicale
            • Aide à la prise du repas si nécessaire`,
        text4: `Aide au lever et au coucher. Soins élémentaires d’hygiène dans la limite des prescriptions médicales`,
        text5: `Petit lavage à la main et lavage du linge en machine qui ne nécessite pas de traitement particulier. Repassage du linge courant, rangement.`
      }
    }
  }
</script>

<style>
.btn-info:hover {
    color: #fff;
    background-color: #364182;
    border-color: none;
}
.btn-info {
    color: #fff;
    background-color: #364182;
    border-color: #117a8b;
}
</style>