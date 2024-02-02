<script>
  import Competence from "$components/Competence.svelte";
  import Contacts from "$components/Contacts.svelte";
  import Fa from "svelte-fa";
  import { faLongArrowDown } from "@fortawesome/free-solid-svg-icons";
</script>

<main>
  <img src="/assets/top-bg.svg" alt="top background" />
  <img src="/assets/bottom-bg.svg" alt="bottom background" />
  <nav>
    <img src="/assets/Logo.svg" alt="logo GTI" />
    <div>
      <a href="#competences">Compétences</a>
      <a href="#fournisseurs">Fournisseurs</a>
      <a href="#clients">Clients</a>
    </div>
  </nav>
  <section class="accueil">
    <div>
      <h1>Gestion technique informatisée</h1>
      <p>
        Depuis 1999, nous apportons un soin à mettre en oeuvre et accompagner nos clients dans l’intégration de systèmes de gestion technique du bâtiment en France et au Bénélux. 
      </p>
    </div>
    <div class="side-accueil">
      <img src="/assets/fournisseurs/trend.png" alt="logo fournisseur trend" />
      <img src="/assets/fournisseurs/wago.png" alt="logo fournisseur wago" />
      <img src="/assets/fournisseurs/distech.png" alt="logo fournisseur distech" />
      <a href="#fournisseurs">Voir d'autres</a>
    </div>
  </section>
  <Contacts />
  <section id="competences">
    <h2>
      Nous travaillons dans <br />
      de nombreux domaines <br />
      pour plusieurs entreprises
    </h2>
  </section>
  <section class="competences">
    <Competence src="/assets/competences/datacenter.png" alt="Datacenter">
      <span slot="title"> Datacenter </span>
      <span slot="paragraph"
        >Assurez le contrôle et suivi des conditions climatique intérieur à l’aide d’automatisme en redondance.</span
      >
    </Competence>
    <Competence
      src="/assets/competences/sports.png"
      alt="tuyauterie sous-terraine de piscine"
    >
      <span slot="title"> Sports et loisirs </span>
      <span slot="paragraph"
        >GTB de complexes aquatiques en passant par l’automatisation des filtrations et la gestion des salle de sport.</span
      >
    </Competence>
    <Competence
      src="/assets/competences/bureaux.png"
      alt="immeubles vue en contre-plongée avec les ciel derriere"
    >
      <span slot="title"> Bureaux </span>
      <span slot="paragraph"
        >Mise à disposition de systèmes permettant aux utilisateurs finaux de contrôler entièrement leur environnement de lieu de travail.</span
      >
    </Competence>
    <Competence
      src="/assets/competences/education.png"
      alt="étudiant lisant un livre dans une bibliothèque moderne"
    >
      <span slot="title"> Éducations </span>
      <span slot="paragraph"
        >De la crèche à l’université accompagner les futures générations dans des bâtiments modernes et efficient via les automatismes du bâtiment.</span
      >
    </Competence>
    <Competence
      src="/assets/competences/sante.png"
      alt="Materiel médical issu d'un hopital"
    >
      <span slot="title"> Santé </span>
      <span slot="paragraph"
        >Système de GTC des bâtiments, pour apporter aux usagers un confort et une aide au pilotage de ce type de bâtiment.</span
      >
    </Competence>
  </section>
  <section id="fournisseurs">
    <h2>
      Nos principaux fournisseurs<br />
      avec qui nous travaillons
    </h2>
  </section>
  <section class="fournisseurs">
    <div>
      <picture><img src="/assets/fournisseurs/trend.png" alt="logo fournisseur trend orange" /></picture>
      <p> Lorem ipsum dolor sit amet, consectetur adipiscing elit. Mauris vestibulum urna at cursus tempus. Ut iaculis, velit ut aliquet pretium, ex tellus maximus risus, rutrum tristique orci nibh sit amet metus.</p>
    </div>
    <div>
      <picture><img src="/assets/fournisseurs/wago.png" alt="logo fournisseur wago vert" /></picture>
      <p> Lorem ipsum dolor sit amet, consectetur adipiscing elit. Mauris vestibulum urna at cursus tempus. Ut iaculis, velit ut aliquet pretium, ex tellus maximus risus, rutrum tristique orci nibh sit amet metus.</p>
    </div>
    <div>
      <picture><img src="/assets/fournisseurs/distech.png" alt="logo fournisseur distech bleu"/></picture>
      <p> Lorem ipsum dolor sit amet, consectetur adipiscing elit. Mauris vestibulum urna at cursus tempus. Ut iaculis, velit ut aliquet pretium, ex tellus maximus risus, rutrum tristique orci nibh sit amet metus.</p>
    </div>
    <div>
      <picture><img src="/assets/fournisseurs/honeywell.png" alt="logo fournisseur honeywell rouge"/></picture>
      <p> Lorem ipsum dolor sit amet, consectetur adipiscing elit. Mauris vestibulum urna at cursus tempus. Ut iaculis, velit ut aliquet pretium, ex tellus maximus risus, rutrum tristique orci nibh sit amet metus.</p>
    </div>
    <div>
      <picture><img src="/assets/fournisseurs/belimo.png" alt="logo fournisseur belimo orange et noir" /></picture>
      <p> Lorem ipsum dolor sit amet, consectetur adipiscing elit. Mauris vestibulum urna at cursus tempus. Ut iaculis, velit ut aliquet pretium, ex tellus maximus risus, rutrum tristique orci nibh sit amet metus.</p>
    </div>
    <div>
      <picture><img src="/assets/fournisseurs/thermokon.svg" alt="logo fournisseur thermokon rouge" /></picture>
      <p> Lorem ipsum dolor sit amet, consectetur adipiscing elit. Mauris vestibulum urna at cursus tempus. Ut iaculis, velit ut aliquet pretium, ex tellus maximus risus, rutrum tristique orci nibh sit amet metus.</p>
    </div>
    <div>
      <picture><img src="/assets/fournisseurs/metz.png" alt="logo fournisseur metz connect bleu foncé et noir" /></picture>
      <p> Lorem ipsum dolor sit amet, consectetur adipiscing elit. Mauris vestibulum urna at cursus tempus. Ut iaculis, velit ut aliquet pretium, ex tellus maximus risus, rutrum tristique orci nibh sit amet metus.</p>
    </div>
    <div>
      <picture><img src="/assets/fournisseurs/KEP.png" alt="logo KEP vert" /></picture>
      <p> Lorem ipsum dolor sit amet, consectetur adipiscing elit. Mauris vestibulum urna at cursus tempus. Ut iaculis, velit ut aliquet pretium, ex tellus maximus risus, rutrum tristique orci nibh sit amet metus.</p>
    </div>
  </section>
  <section id="clients">
    <h2>Nos clients installateurs <br />
       qui nous font confiance</h2>
  </section>
  <section class="clients">
      <div>
        <img src="/assets/installateurs/bail.png" alt="logo effet d'o, Chauffage sanitaire climatisation" />
        <img src="/assets/installateurs/brunet.png" alt="logo brunet alpha clima, l'offre multitechnique de proximité, Ortec group" />
        <img src="/assets/installateurs/dalkia.png" alt="logo dalkia, groupe edf" />
        <img src="/assets/installateurs/delannoydewailly.png" alt="logo delannoy dewailly" />
        <img src="/assets/installateurs/effetdo.png" alt="logo effet d'o, Chauffage sanitaire climatisation" />
        <img src="/assets/installateurs/engie.png" alt="logo engie solutions" />
        <img src="/assets/installateurs/herve-thermique.png" alt="logo brunet alpha clima, l'offre multitechnique de proximité, Ortec group" />
        <img src="/assets/installateurs/spie.png" alt="logo spie, l'offre multitechnique de proximité, Ortec group" />
        <img src="/assets/installateurs/tem.png" alt="logo effet d'o, Chauffage sanitaire climatisation" />
      </div>
  </section>
  <footer>
    <img src="/assets/Logo.svg" alt="logo GTI" />
    <a href="google.com" target="_blank">Mentions légales</a>
    <a href="google.com" target="_blank">Conditions générales</a>
    <a href="mailto:stephane.eckman@gestion-technique-informatisee.fr">Nous contacter</a>
  </footer>
</main>

<style>
  :global(*) {
    font-family: "Prompt", sans-serif;
  }

  :global(html) {
    scroll-behavior: smooth;
  }

  :global(body){
    overflow-x: hidden;
    margin: 0;
  }

  main > img:first-of-type {
    z-index: -1;
    position: absolute;
    width: 100%;
    height: 180vh;
    max-height: 1437px;
    left: 0;
  }

  main > img:last-of-type {
    z-index: -1;
    position: absolute;
    width: 100%;
    left: 0;
    top: 340%;
  }

  nav {
    display: flex;
    flex-direction: row;
    justify-content: space-between;
    padding: 50px;
    padding-left: 100px;
  }

  nav img {
    width: 171px;
    height: 112px;
  }

  nav a {
    color: #002b3d;
    display: inline-block;
    margin-bottom: 0;
    background-image: linear-gradient(#002b3d 0 0);
    background-position: 0 100%;
    background-size: 0% 2px;
    background-repeat: no-repeat;
    transition: background-size 0.3s, background-position 0s 0.3s;
    margin-left: 25px;
    margin-right: 25px;
    font-size: 1.6em;
    font-weight: 200;
    text-decoration: none;
  }

  nav a:hover {
    background-position: 100% 100%;
    background-size: 100% 2px;
  }

  nav div {
    display: flex;
    height: 40px;
  }

  section p {
    font-size: 32px;
    font-weight: 300;
  }

  h1 {
    color: #002b3d;
    font-size: 38px;
    font-weight: 700;
  }

  .accueil {
    padding-left: 100px;
    padding-top: 50px;
    margin-bottom: 60px;
    display: flex;
  }

  .accueil div:first-of-type {
    width: 49%;
  }

  .side-accueil {
    position: relative;
    width: 50%;
    margin-left: 20px;
  }

  .side-accueil img {
    width: 274px;
  }

  .side-accueil > img:nth-child(1) {
    position: absolute;
    top: 0;
    left: 10%;
  }

  .side-accueil > img:nth-child(2) {
    position: absolute;
    top: 25%;
    right: 5%;
  }

  .side-accueil > img:nth-child(3) {
    position: absolute;
    bottom: 15%;
    left: 5%;
  }

  .side-accueil a {
    font-size: 25px;
    position: absolute;
    bottom: 0;
    right: 10%;
    color: #002b3d;
    text-decoration: none;
    background-image: linear-gradient(#002b3d 0 0);
    background-position: 0 100%;
    background-size: 0% 2px;
    background-repeat: no-repeat;
    transition: background-size 0.3s, background-position 0s 0.3s;
  }

  .side-accueil a:hover {
    background-position: 100% 100%;
    background-size: 100% 2px;
  }

  h2 {
    font-size: 34px;
    font-weight: 400;
    text-align: center;
    position: absolute;
    color: #002b3d;
  }

  #competences {
    position: relative;
    height: 200px;
    color: #002b3d;
    margin-bottom: 10px;
  }

  #competences h2 {
    top: 0;
    left: 130px;
  }

  .competences {
    display: flex;
    flex-wrap: wrap;
    justify-content: center;
    align-items: center;
    margin-bottom: 300px;
  }

  #fournisseurs {
    position: relative;
    height: 200px;
    color: #002b3d;
  }

  #fournisseurs h2 {
    top: 0;
    left: 100px;
    color: #002b3d;
  }

  .fournisseurs {
    display: flex;
    flex-wrap: wrap;
    justify-content: center;
    padding: 50px;
    margin-bottom: 40px;
  }
  
  .fournisseurs div {
    display: flex;
    position: relative;
    justify-content: center;
    align-items: center;
    transform: translateY(0);
    max-width: 450px;
  }

  .fournisseurs img {
    height: 110px;
  }

  picture {
    border-radius: 10px;
    box-sizing: border-box;
    margin: 50px;
    transition: all 0.3s;
    background-color: rgb(255, 255, 255);
    border: 1px solid #002b3d;
    padding: 10px;
    z-index: 1;
    display: block;
    position: relative;
  }

  picture::after {
    content: "";
    position: absolute;
    bottom: -2px;
    left: 50%;
    transform: translateX(-50%);
    width: 300px;
    height: 4px;
    z-index: 20000;
    background-color: white;
    opacity: 0;
  }
  
  picture:hover::after {
    opacity: 1;
  }

  .fournisseurs p {
    text-align: center;
    position: absolute;
    bottom: 25%;
    transform: translateY(0);
    transition: all 0.3s;
    color: #002b3d;
    background-color: rgb(255, 255, 255);
    border-radius: 0;
    height: 100px;
    width: 300px;
    font-size: 1.4em;
    border: 1px solid #002b3d;
    border-top: none;
    font-size: 0.8em;
  }


  .fournisseurs picture:hover + p {
    border-radius: 0 0 10px 10px;
    transform: translateY(100px);
  }

  picture:hover {
    transform: translateY(-23px);
  }

  #clients {
    height: 200px;
  }

  #clients h2 {
    width: 55%;
  }

  .clients div{
    display: flex;
    align-items: center;
    justify-content: center;
    flex-direction: row;
    flex-wrap: wrap;
    padding: 0 50px;
  }

  .clients img {
    width: 186px;
    margin-bottom: 20px;
    padding: 0 30px;
  }

  footer {
    background-color: rgb(192, 192, 192);
    left: 0;
    position: absolute;
    width: 100%;
    height: 80px;
    display: flex;
    justify-content: center;
    align-items: center;
  }

  footer img {
    height: 80%;
    margin-right: 20px;
  }

  footer a {
    margin-left: 20px;
    margin-right: 20px;
    color: #002b3d;
    text-decoration: none;
  }

  @media screen and (max-width: 1246px) {
    .side-accueil img:nth-child(2) {
      top: 30%;
    }

    main > img:first-of-type {
      z-index: -1;
      position: absolute;
      width: 100%;
      height: 220vh;
      max-height: 1437px;
      left: 0;
    }

    main > img:last-of-type {
      z-index: -1;
      position: absolute;
      width: 100%;
      left: 0;
      top: 340%;
    }

  }

  @media screen and (max-width: 1000px) {
    .side-accueil {
      display: none;
    }

    .accueil div:first-of-type {
      width: 100%;
      padding-right: 10%;
    }

    nav {
      align-items: center;
    }

    #clients h2{
      left: 50%;
      transform: translateX(-50%);
    }
  }

  @media screen and (max-width: 830px) {
    nav {
      flex-direction: column;
      justify-content: center;
      align-items: center;
      padding: 50px;
    }

    nav a {
      padding-top: 5%;
    }
  }

  @media screen and (max-width: 630px) {
    nav div {
      margin-left: 5%;
      margin-right: 5%;
    }

    .accueil p{
      font-size: 1.2em;
    }

    nav a {
      padding-top: 5%;
    }

    h2 {
      font-size: 1.6em;
    }


  }
  
  @media screen and (max-width: 550px) {
    nav div {
      flex-direction: column;
      height: 100%;
    }

    nav {
      flex-direction: row;
      align-items: center;
      padding-top: 20px;
      padding-bottom: 0;
    }

    nav a {
      margin: 0;
    }

    nav a:first-of-type {
      padding: 0;
    }

    .fournisseurs img {
      height: 80px;
    }

    .fournisseurs p{
      font-size: 0.7em;
      width: 200px;
    }

    .fournisseurs picture:hover + p {
      border-radius: 0 0 10px 10px;
      transform: translateY(80px);
    }

    .clients {
      align-items: center;
      flex-direction: column;
    }

    .clients div:first-of-type{
      margin-bottom: 40px;
    }

    footer a{
      font-size: 0.7em;
    }
  }
</style>
