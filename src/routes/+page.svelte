<script>
	import SectionCard from './../lib/components/SectionCard.svelte';
	import ButtnSVG from './../lib/components/ButtnSVG.svelte';
</script>

  <div class="hero">
    <img src="/images/hero.png" alt="" />
    <h1>FOSTER APP</h1>
    <p>Domov v srdci, pomoc na dosah.</p>
    <a href="/login"><ButtnSVG class="tlacitko">Začít</ButtnSVG></a>

  </div>
  
  <div class="sections">
    <SectionCard img="/images/support.png" head="Podpora na každém kroku">Nástroje, které pomáhají dětem lépe <br> zvládat každodenní situace</SectionCard>
    <SectionCard img="/images/learn.png" head="Učení a rozvoj">Zdroje, které podporují vzdělání, <br>osobní růst a sebevědomí</SectionCard>
    <SectionCard img="/images/community.png" head="Propojení s komunitou">Zdroje, které propojují rodiny, pečovatele i děti.</SectionCard>
    <SectionCard img="/images/goals.png" head="Společně..">můžeme udělat krok ke světu, kde <br> každý má dítě šanci na šťastný život</SectionCard>
    <SectionCard img="/images/pani.png" head="Poradce ve vaší kapse">Náš poradce v aplikaci je tu proto,<br> aby vám poskytl pomoc a podporu <br>kdykoliv ji budete potřebovat.</SectionCard>
  </div>

  <div class="colum">
    <div class="text-colum">
      <p>Podpora, kterou si zasloužíš. <br> Budoucnost, kterou můžeš tvořit.</p>
      <a href="/login"><ButtnSVG class="tlacitko">DOMUS</ButtnSVG></a>
    </div>
    <div class="img-colum">
      <img src="/images/4section.png" alt="">
    </div>
  </div>

<div class="footer">
  <p>Foster app <br> TechTower, 301 00 Plzeň <br>
    IČO: xxxxxxxx <br>
    Číslo účtu: xx-xxxxxxxxxx/xxxx <br>
    ID datové schránky: xxxxxx <br>
    Kontakt: <a href="mailto:info@fosterapp.cz">info@fosterapp.cz</a>
  </p>
</div>
  
  <style>
    .colum{
      display: flex;
      padding-left: 25px;
      padding-bottom: 20px;
      gap: 10px;
      padding-top: 35px;
    }

    .text-colum p{
      font-weight: bold;
      color: #333;
      font-family: Outfit;
      font-size: 12px;
      font-weight: 900;
      padding-bottom: 25px;
    }

    a{
      text-decoration: none;
    }
    
    .sections{
      background-image: url('/images/backgroud.png');
    }
    
    /* Hero Section */
    .hero {
      text-align: center;
      padding: 40px 20px;
      background-color: #fdf3f7;
      
    }

    .hero img {
      width: 100%;
      max-width: 300px;
      margin: 0 auto 20px;
    }
  
    .hero h1 {
        font-family: "Outfit", sans-serif;
        font-weight: 900;
        font-size: 32px;
    }
  
    .hero p {
        font-family: "Outfit", sans-serif;
        font-weight: 900;
        font-size: 16px;
    }
  
   
    .social-media {
    display: flex;
    justify-content: center;
    gap: 20px;
    margin: 20px 0;
    }

  .social-media img {
    width: 50px;
    height: 50px;
    justify-content: center;
  }

  .footer {
    background-color: #4C328A;
    color: white;
    padding: 20px;
    text-align: left;
    border-top: 6px solid #E44F95;
  }

  .footer p {
    color: white;
    font-family: Outfit;
    font-size: 10px;
    font-weight: 500;
    line-height: 7.56px;
    text-align: left;
    text-underline-position: from-font;
    text-decoration-skip-ink: none;
    line-height: 15px;
  }
  .footer a {
    color: white;
    text-decoration: none;
    font-weight: bold;
  }

</style>