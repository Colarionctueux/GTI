<script>
    import { faPhoneSquareAlt, faEnvelope, faLongArrowRight} from "@fortawesome/free-solid-svg-icons";
    import { faLinkedin } from "@fortawesome/free-brands-svg-icons";
    import Fa from "svelte-fa";
    function sendemail(){
        // @ts-ignore
        window.location = "mailto:stephane.eckman@gestion-technique-informatisee.fr"
    }
</script>

<main>
    <div>
        <h2>Contacts</h2>
        <p> <Fa icon={faPhoneSquareAlt}/> 03 20 98 17 33</p>
        <p> <Fa icon={faEnvelope}/> stephane.eckman@gestion-technique-informatisee.fr</p>
        <p> <Fa icon={faLinkedin}/> https://fr.likedin/je-ne-sais-pas</p>
    </div>
    <div>
        <button>Démonstration</button>
        <button on:click={sendemail}>Contacter<span><Fa icon={faLongArrowRight} /></span></button>
    </div>
</main>
<style>
    main{
        border-radius: 52px;
        border: 2px solid #0B8FB8;
        height: 186px;
        margin: 5%;
        margin-top: 1%;
        margin-bottom: 220px;
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
        font-size: 1.3em;
    }

    div:first-of-type{
        padding-left: 50px;
        width: 50%;
    }
    
    div:last-of-type{
        border-left: 1.6px solid rgba(0, 0, 0, 14%);
        display: flex;
        justify-content: space-evenly;
        align-items: center;
        width: 50%;
        height: 80%;
    }
    
    button{
        font-size: 1.3em;
        background-size: 100% 200%;
        border: 2px solid #0B8FB8;
        border-radius: 10px;
        height: 67px;
        width: 40%;
        font-weight: 200;
        box-shadow: 0 4px 6px rgba(0, 0, 0, 0.2);
        transition: all .3s ease;
    }

    button:last-of-type{
        background-image: linear-gradient(to top, #0B8FB8 50%, white 50%);
        color: #0B8FB8;
    }

    button:first-of-type{
        background-image: linear-gradient(to bottom, #0B8FB8 50%, white 50%);
        color: white;
    }

    span{
        margin-left: 15px;
    }

    button:first-of-type:hover{
        background-position: 0 -100%;
        box-shadow: 2px 6px 10px rgba(0, 0, 0, 0.2);
        color: #0B8FB8;
    }

    
    button:last-of-type:hover{
        background-position: 0 -100%;
        box-shadow: 2px 6px 10px rgba(0, 0, 0, 0.2);
        color: #ffffff;
    }

    @media screen and (max-width : 1030px){
        p{
            font-size: .9em;
        }
    }

    @media screen and (max-width : 1000px){
        div:last-of-type{
            flex-direction: column;
            gap: 20px;
        }

        button{
            width: 75%;
        }

        p{
            padding-top: 5px;
        }
    }

</style>