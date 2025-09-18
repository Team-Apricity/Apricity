<script>
  import CardDetails from "../shared/CardDetails.svelte";
</script>

<div class="Cards">
<CardDetails name="Hiba Karima" job="Front-End Developer" Insta_User="Hiba Karima" GitHub_User="HibaKarima" 
  LinkedIn_User="Hiba Karema" GitHub_Url="https://github.com/HibaKarima" Insta_Url="https://www.instagram.com/hibakarima810?igsh=dXJpcGlrcmpvOTM=" LinkeIn_Url="" Image="Images/Hiba.png"/>

<CardDetails name="Malek Rostum" job="Back-End Developer" Insta_User="Malek Rostum" GitHub_User="NonSense-U" 
  LinkedIn_User="Malek Rostum" GitHub_Url="https://github.com/NonSense-U" Insta_Url="https://www.instagram.com/malekrostum?igsh=dXRuazB4ZGQ0MG82" LinkeIn_Url="" Image="Images/Malek.png"/>

<CardDetails name="Ghena Dobbo" job="UI \ UX  Designer" Insta_User="Ghena Dobbo" GitHub_User="GhenaDobbo" 
  LinkedIn_User="Ghena Dobbo" GitHub_Url="https://github.com/GhenaDobbo" Insta_Url="https://www.instagram.com/_.ghena.__?igsh=MTA5MGUzMWxzbW81dQ==" LinkeIn_Url="" Image='Images/Ghena.png'/>

<CardDetails name="Hussein Mahfoud" job="Front-end Developer" Insta_User="Hussein Mahfoud" GitHub_User="hussein0-0" 
  LinkedIn_User="Hussein Mahfoud" GitHub_Url="https://github.com/hussein0-0" Insta_Url="https://www.instagram.com/hussein_mahfoud74?igsh=MXhlYmY3anliNXhxZw==" LinkeIn_Url="" Image="Images/Hussein.png"/>   

  <CardDetails name="Hassan Shaaban" job="Mobile Developer" Insta_User="Hassan Shaaban" GitHub_User="hassanShaaban" 
  LinkedIn_User="Hassan Shaaban" GitHub_Url="https://github.com/hasanShaaban" Insta_Url="https://www.instagram.com/hasan_a_shaaban?igsh=MWM3cnJhbWQ2cThqcg==" LinkeIn_Url="#" Image="Images/hasan.png"/>
</div>

<style>
.Cards{
  background-color: white;
    padding: 7vw 7vw;
    display: flex;
    justify-content: space-evenly;
    overflow: hidden;
    flex-wrap: wrap;
    gap: 3vw;
    margin: 0;
}

/* Tablet styles */
@media (max-width: 1024px) {
    .Cards {
        padding: 5vw;
        gap: 2.4vw;
    }
}

/* Mobile styles */
@media (max-width: 480px) {
    .Cards {
        padding: 7vw 2vw;
        gap: 1vw;
    }
}
</style>