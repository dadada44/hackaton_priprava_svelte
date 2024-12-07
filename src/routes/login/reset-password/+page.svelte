
<div>
    <h2><strong>Zapomenuté heslo</strong></h2>
    <p class = "prvni"><strong>Zadejte svůj e-mail a my vám<br>pošleme odkaz, abyste se mohli<br>dostat zpět ke svému učtu</strong></p>
        <label>
            E-mail
            <input type="email" placeholder="Zadejte email"/>
        </label>
        <button type="submit"><strong>Změnit heslo</strong></button>
        <a href="/login/new-regist" class="druhy">Nová registrace</a>

    <img src="/images/bottom.png" alt="Obrázek" />
</div>

<style>
    .prvni{
        font-size: 14px;
        text-align: center;
    }
    .druhy{
        text-align: left;
        font-size: 12px;
    }
    *{
        font-family: "Outfit";
    }

    img {
        display: block;
        margin: 20px auto;
        max-width: 100%;
    }

    h2 {
        text-align: center;
        font-size: 22px;
    }

    label {
        display: block;
        margin-bottom: 5px;
        font-weight: bold;
    }

    input {
        width: 95%;
        padding: 10px;
        margin-bottom: 20px;
        border: 2px solid #000000;
        border-radius: 6px;
        box-sizing: border-box;
    }

    button {
        display: block;
        width: 95%;
        padding: 10px;
        background-color: #51128b;
        color: white;
        border: none;
        cursor: pointer;
        font-size: 18px;
        border-radius: 8px;
    }

    button:hover {
        background-color: #ef9dc3;
    }
</style>