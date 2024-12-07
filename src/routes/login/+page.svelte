<div class= "prvni">
    <h1>LOGIN</h1>
        <label class="email">
            E-mail
            <input type="email" placeholder="Zadejte email"/>
        </label>
        <label>
            Heslo
            <input type="password" placeholder="Zadejte heslo" />
        </label>
        <button type="submit"><strong>Přihlásit se</strong></button>
        <a href="/login/new-regist">Nová registrace</a>
        <a href="/login/reset-password">Zapomenuté heslo</a>

    <img src="/images/bottom.png" alt="Obrázek" />
</div>

<style>
    *{
        font-family: "Outfit";
    }
    p{
        font-size: 14px;
        text-align: left;
    }

    img {
        display: block;
        margin: 0;
        max-width: 100%;
    }

    h1 {
        text-align: center;
        font-size: 25px;
    }

    label {
        display: block;
        margin-bottom: 5px;
        font-weight: bold;
    }
    .email{
        width: 300px;
        height: 70px;
        top: 209px;
        left: 45px;
        gap: 0px;
        border: 1px 0px 0px 0px;
        opacity: 0px;

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