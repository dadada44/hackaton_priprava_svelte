<script>
    // Získání atributů z props s výchozími hodnotami
    let { label = "Nadpis", children } = $props();
</script>

<div class="card">
    <div class="card-bg"></div> <!-- Přidání pozadí s clip-path -->
    <h2 class="card-title">{label}</h2>
    <p class="card-text">
        {@render children()} <!-- Vykreslení obsahu (children) -->
    </p>
</div>

<style lang="scss">
    .card {
        position: relative;
        width: 100%;
        max-width: 350px; /* Maximální šířka kartičky */
        margin: 20px auto; /* Mezera mezi kartičkami */
        padding: 20px;
        border-radius: 12px; /* Zaoblení rohů */
        background-color: transparent;
        overflow: hidden;
        background-color: #54473F;
        border-radius: 32px;
        transition: all 0.5s ease; /* Hladká animace pro hover */
    }

    /* Sunrise pozadí */
    .card-bg {
        position: absolute;
        top: 0;
        left: 0;
        width: 100%;
        height: 100%;
        background: linear-gradient(135deg, #9A7E6F, #9A7E6F); /* Sunrise barvy */
        clip-path: circle(0% at 50% 50%); /* Výchozí tvar je kruh s 0% */
        transition: clip-path 0.7s ease-out;
    }

    .card:hover .card-bg {
        clip-path: circle(150% at 50% 50%); /* Roztažení kruhu na celý obsah */
    }

    .card:hover {
        border-radius: 64px 44px 15px 96px;
        box-shadow: #54473F 0px 4px 16px, #54473F 0px 8px 32px;
        transform: translateY(-5px); /* Zvednutí kartičky při hoveru */
    }

    /* Styly pro nadpis kartičky */
    .card-title {
        position: relative;
        font-size: 1.8rem; /* Velikost písma pro nadpis */
        font-weight: bold; /* Tučné písmo pro nadpis */
        color: #E9EED9; /* Bílá barva pro text */
        margin-bottom: 10px; /* Mezera pod nadpisem */
        text-transform: uppercase; /* Velká písmena pro nadpis */
        letter-spacing: 1px; /* Rozteč písmen */
        z-index: 1; /* Zajištění, že text je nad pozadím */
    }

    /* Styly pro text kartičky */
    .card-text {
        position: relative;
        font-size: 1rem; /* Velikost textu pro obsah */
        color: #E9EED9; /* Bílá barva textu */
        line-height: 1.6; /* Větší řádkování pro lepší čitelnost */
        margin-top: 10px; /* Mezera nad obsahem */
        text-align: justify; /* Zarovnání textu do bloku */
        z-index: 1; /* Zajištění, že text je nad pozadím */
    }
</style>
