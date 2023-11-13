<script>
    import { faPhoneSquareAlt, faEnvelope, faUser } from "@fortawesome/free-solid-svg-icons";
    import Fa from "svelte-fa";
</script>

<main>
    <div>
        <h2>Contacts</h2>
        <p> <Fa icon={faPhone}/>03 20 98 17 33</p>
        <p>stephane.eckman@gestion-technique-informatisee.fr</p>
        <p>https://fr.likedin/je-ne-sais-pas</p>
    </div>
    <div />
</main>
<style>
    main{
        border-radius: 52px;
        border: 2px solid #0B8FB8;
        height: 186px;
        margin: 5%;
        margin-bottom: 0;
        background-color: white;
    }

    h2{
        font-family: "Prompt", sans-serif;
        font-weight: 200;
    }

    p{
        font-family: "Prompt", sans-serif;
        font-weight: 200;
    }

    main>div:first-of-type{
        padding-left: 50px;
    }


</style>