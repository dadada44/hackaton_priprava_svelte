<script>
	import ButtnSVG from './../lib/components/ButtnSVG.svelte';
    // Pokud chcete, můžete importovat data dynamicky
    const sections = [
      {
        image: '/images/support.png',
        title: 'Podpora na každém kroku',
        description: 'Nástroje, které pomáhají dětem lépe zvládat každodenní situace.'
      },
      {
        image: '/images/learn.png',
        title: 'Učení a rozvoj',
        description: 'Zdroje, které podporují vzdělání, osobní růst a sebevědomí.'
      },
      {
        image: '/images/community.png',
        title: 'Propojení s komunitou',
        description: 'Zdroje, které propojují rodiny, pečovatele i děti.'
      }
    ];
  </script>

  <div class="hero">
    <img src="/images/hero.png" alt="Hero Image" />
    <h1>FOSTER APP</h1>
    <p>Domov v srdci, pomoc na dosah.</p>
    <ButtnSVG class="tlacitko">Začít</ButtnSVG>
  </div>
  
  <div class="sections">
    {#each sections as section}
      <div class="section">
        <img src={section.image} alt={section.title} />
        <h2>{section.title}</h2>
        <p>{section.description}</p>
      </div>
    {/each}
  </div>
  
  <style>
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
  
    .cta-button {
      background: linear-gradient(135deg, #8e44ad, #ec6ead);
      color: white;
      border: none;
      padding: 10px 20px;
      font-size: 16px;
      font-weight: bold;
      border-radius: 25px;
      cursor: pointer;
    }
  
    /* Sections */
    .sections {
      padding: 20px;
    }
  
    .section {
      text-align: center;
      margin-bottom: 40px;
    }
  
    .section img {
      width: 100%;
      max-width: 150px;
      margin: 0 auto 20px;
    }
  
    .section h2 {
      font-size: 18px;
      margin-bottom: 10px;
    }
  
    .section p {
      font-size: 14px;
      color: #555;
    }
  </style>