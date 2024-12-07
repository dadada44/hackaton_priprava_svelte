<script>
    // Definice props a jejich destrukturalizace
    let { img, head, children } = $props();
  </script>
  
  <div class="section-support">
    <img src={img} alt={head} />
    <h2>{head}</h2>
    <p>{@render children()}</p>
  </div>
  
  <style>
    .section-support {
      display: flex;
      justify-content: center;
      align-items: center;
      flex-direction: column;
      width: 100%;
    }
    .section-support img {
      max-width: 300px;
    }
    .section-support h2 { 
      font-size: 25px;
      font-family: "Outfit", sans-serif;
      font-weight: 900;
    }
    .section-support p {
      font-size: 15px;
      color: #666;
      font-family: "Outfit", sans-serif;
      font-weight: 900;
    }
  </style>
  