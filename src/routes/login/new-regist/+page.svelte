

<div>
    <h1>REGISTRACE</h1>
    <label>
        Nickname
        <input type="text" placeholder="Zadejte nickname" />
    </label>
    <label>
        E-mail
        <input type="email"placeholder="Zadejte email" />
    </label>
    <label>
        Heslo
        <input type="number"  placeholder="Zadejte heslo" />
    </label>
    <label>
        Potvrzeni hesla
        <input type="password"  placeholder="Zadejte podtvrzeni " />
    </label>
    <button type="submit"><strong>Vytvořit učet</strong></button>
    <a href="/login">Již máte učet?</a>
    <img src="/images/bottom.png" alt="Obrázek"/>
  </div>
  
  <style>
    img{
        display:block;
        margin: 20px auto;
        max-width: 100%;
    }
    h1{
        font-family: "Outfit";
        text-align: center;
        font-size: 25px;
    }
    p{
        font-family: "Outfit";
        text-align: left;
        font-size: 12px;
    }
  
    label {
        display: block;
        margin-bottom: 10px;
        font-weight: bold;
        font-family: "Outfit";
    }
  
    input {
        width: 100%;
        padding: 8px;
        margin-bottom: 20px;
        border: 2px solid #000000;
        border-radius: 6px;
        box-sizing: border-box;
        font-family: "Outfit";
    }
  
    button {
        display: block;
        width: 100%;
        padding: 10px;
        background-color: #51128b;
        color: white;
        border: none;
        cursor: pointer; 
        font-size: 18px;
        border-radius: 8px;
        font-family: "Outfit";
    }
  
    button:hover {
        background-color: #ef9dc3;
    }
  </style>
    