<script>
    // Získání atributů z `$props`, s výchozími hodnotami
    let { href = "#", color = "default", children } = $props();

    // Dynamická třída
    let Button_class = `${color} button`;
</script>

<a {href} class={Button_class}>
    {@render children()} <!-- Správné použití {@render} pro vykreslení children -->
</a>

<style lang="scss">
    .button {
        max-width: 85px;
        width: 100%;
        text-align: center;
        text-decoration: none;
        padding: 10px;
        margin-top: 25px;
        background-color: #fff; /* Bílá barva pozadí */
        border-radius: 12px; /* Zaoblení rohů */
        transition: all 0.3s ease; /* Hladká animace pro hover */
    }

    .button:hover {
        transform: translateY(-5px); /* Zvednutí kartičky při hoveru */
        box-shadow: #54473F 0px 4px 16px, #54473F 0px 8px 32px;
    }


    .default {
        background-color: #ccc;
        color: #000;
    }
    .brown {
        background-color: #9A7E6F;
        color: #E9EED9;
    }
</style>