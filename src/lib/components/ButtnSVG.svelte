<script>
    // Přijímáme children pro obsah uvnitř hlavního divu
    const { children } = $props();
  </script>
  
  <div class="container">
    <div class="content">
      {@render children()}
    </div>
  </div>
  
  <style lang="scss">
    .container {
      position: relative;
      width: 100%; /* Dynamická šířka */
      height: auto;
      aspect-ratio: 134 / 56; /* Poměr stran SVG */
      overflow: hidden; /* Zabrání přetečení */
      max-width: 140px;
      margin: auto;
      display: flex;
      justify-content: center;
      align-items: center;
      cursor: pointer;

    }
  
    .container::after {
      content: '';
      position: absolute;
      top: 0;
      left: 0;
      width: 100%;
      height: 100%;
      background: linear-gradient(90deg, #E44F95 0%, #4C328A 100%);
      clip-path: path('M133.5 33.5C133.5 48.6878 102.555 56 65 56C27.4446 56 0.5 31.6878 0.5 16.5C0.5 1.31217 45.4446 0.5 83 0.5C120.555 0.5 133.5 18.3122 133.5 33.5Z');
      z-index: 1; /* SVG je za obsahem */
    }
  
    .content {
        position: relative;
        z-index: 10; /* Obsah je viditelný nad SVG */
        display: flex;
        align-items: center;
        justify-content: center;
        height: 100%; /* Obsah se přizpůsobí velikosti divu */
        padding: 1rem;
        text-align: center;
        color: #fff; /* Příklad kontrastu proti gradientu */
        font-family: "Outfit", sans-serif;
        font-weight: 900;
        font-size: 24px;
    }
</style>
  