<script>
    import { faPhoneSquareAlt, faEnvelope, faLongArrowRight} from "@fortawesome/free-solid-svg-icons";
    import { faLinkedin } from "@fortawesome/free-brands-svg-icons";
    import Fa from "svelte-fa";
</script>

<main>
    <div>
        <h2>Contacts</h2>
        <p> <Fa icon={faPhoneSquareAlt}/> 03 20 98 17 33</p>
        <p> <Fa icon={faEnvelope}/> stephane.eckman@gestion-technique-informatisee.fr</p>
        <p> <Fa icon={faLinkedin}/> https://fr.likedin/je-ne-sais-pas</p>
    </div>
    <div>
        <button>Demander un devis</button>
        <button>Contacter  <span><Fa icon={faLongArrowRight} /></span></button>
    </div>
</main>
<style>
    main{
        border-radius: 52px;
        border: 2px solid #0B8FB8;
        height: 186px;
        margin: 5%;
        margin-top: 1%;
        margin-bottom: 0;
        background-color: white;
        display: flex;
        align-items: center;
    }

    h2{
        font-family: "Prompt", sans-serif;
        font-weight: 200;
        margin-bottom: 13px;
        margin-top: 0;
    }
    
    p{
        font-family: "Prompt", sans-serif;
        font-weight: 200;
        margin : 0;
    }

    main>div:first-of-type{
        padding-left: 50px;
        width: 50%;
    }

    main>:first-of-type p{
        font-size: 1.3em;
    }
    
    main div:last-of-type{
        border-left: 1.6px solid rgba(0, 0, 0, 14%);
        display: flex;
        justify-content: space-evenly;
        align-items: center;
        width: 50%;
        height: 80%;
    }
    
    button{
        font-size: 1.3em;
        background-color: white;
        border: 2px solid #0B8FB8;
        border-radius: 10px;
        height: 67px;
        width: 258px;
        font-weight: 200;
        color: #0B8FB8;
        box-shadow: 0 4px 6px rgba(0, 0, 0, 0.2);
    }

    main div:last-of-type button:first-of-type{
        background-color: #0B8FB8;
        color: white;
    }

    span{
        margin-left: 15px;
    }

</style>