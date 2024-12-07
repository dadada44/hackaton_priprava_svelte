<script>
	import ButtnSVG from './../lib/components/ButtnSVG.svelte';
</script>

  <div class="hero">
    <img src="/images/hero.png" alt="" />
    <h1>FOSTER APP</h1>
    <p>Domov v srdci, pomoc na dosah.</p>
    <a href="/login"><ButtnSVG class="tlacitko">Začít</ButtnSVG></a>

  </div>
  
  <div class="sections">
    <div class="section-support">
      <img src='/images/support.png' alt="" />
      <h2>Podpora na každém kroku</h2>
      <p>Nástroje, které pomáhají dětem lépe zvládat každodenní situace.</p>
    </div>
    <div class="section-learn">
      <img src='/images/learn.png' alt="" />
      <h2>Učení a rozvoj</h2>
      <p>Zdroje, které podporují vzdělání, <br>osobní růst a sebevědomí.</p>
    </div>
    <div class="section-community">
      <img src='/images/community.png' alt="" />
      <h2>Propojení s komunitou</h2>
      <p>Zdroje, které propojují rodiny, pečovatele i děti.</p>
    </div>
    <div class="section-goals">
      <img src='/images/goals.png' alt="" />
      <h2>Společně můžeme udělat krok ke světu, kde každý má dítě šanci na šťastný život.</h2>
    </div>
    <div class="section-pani">
      <img src='/images/pani.png' alt="" />
      <h2>Poradce ve vaší kapse</h2>
      <p>Náš poradce v aplikaci je tu proto, aby vám poskytl pomoc a podporu kdykoliv ji budete potřebovat. Ať už máte otázky, potřebujete radu, nebo jen někoho, kdo vám porozumí, poradce je spolehlivý průvodce na vaší cestě.</p>
    </div>
  </div>

<div class="container">
  <p>Podpora, kterou si zasloužíš. Budoucnost, kterou můžeš tvořit.</p>
  <div class="social-media">
    <p>Jsme na sociálních médiích:</p>
    <ButtnSVG>
      <img src="/images/facebook.png" alt="Facebook" />
      <img src="/images/youtube.png" alt="YouTube" />
      <img src="/images/instagram.png" alt="Instagram" />
    </ButtnSVG>
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

    a{
      text-decoration: none;
    }
    
    .sections{
      background-image: url('/images/backgroud.png');
    }

    .section-support{
      margin: 35px;
      width:50vw;
      float: right;
      text-align: right;
    }
    .section-learn{
      margin: 35px;
    }
    .section-community{
      margin: 35px;
      width:50vw;
      float: right;
      text-align: right;
    }

    .section-goals{
      padding: 20px;
      text-align: center;
    }

    .section-pani{
      padding: 20px;
      text-align: center;
    }

    .logo {
      font-weight: bold;
      font-size: 18px;
    }
  
    .menu-icon {
      width: 30px;
      height: 30px;
      background: white;
      border-radius: 50%;
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

  
    img {
      width: 100%;
      max-width: 150px;
    }
  
    h2 {
      font-family: "Outfit", sans-serif;
      font-weight: 900;
      font-size: 14px;
      margin-left: 20px;
    }
  
    p {
      font-family: "Outfit", sans-serif;
      font-weight: 900;
      font-size: 10px;
      color: #686868;
      margin-left: 20px;
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
  }

  .footer p {
    color: white;
    font-family: Outfit;
    font-size: 6px;
    font-weight: 900;
    line-height: 7.56px;
    text-align: left;
    text-underline-position: from-font;
    text-decoration-skip-ink: none;
  }
  .footer a {
    color: white;
    text-decoration: none;
    font-weight: bold;
  }

</style>