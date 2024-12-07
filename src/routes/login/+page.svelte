<div class="login">
    <h1>LOGIN</h1>
    <label class="email">
        E-mail
        <input type="email">
    </label>
    <label>
        Heslo
        <input type="password">
    </label>
    <button type="submit"><strong>Přihlásit se</strong></button>
    <div>
        <a href="/login/new-regist">Nová registrace</a>
        <a href="/login/reset-password">Zapomenuté heslo</a>
    </div>
</div>
   <img src="/images/bottom.png" alt="Obrázek" />
<style lang="scss">
    *{
        font-family: "Outfit";
    }
    /*

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
    }*/
    .login{
        display: flex;
        flex-direction: column;
        justify-content: center;
        align-items: center;
        max-width: 600px;
        width: 100%;
        padding: 30px;
        box-sizing: border-box;
        gap: 14px;
        margin: auto;

        button{
            width: 100%;
            height: 50px;
            border-radius: 10px;
            background-color: #4C328A;
            color: white;
            border: none;
            cursor: pointer;
        }

        label{
            display: flex;
            flex-direction: column;
            width: 100%;
            gap: 4px;
            font-size: 14px;
            font-weight: 500;

            input{
                height: 50px;
                border-radius: 10px;
                padding: 0 10px;
                border: 1.5px solid black;
            }
        }

        div{
            display: flex;
            justify-content: space-between;
            width: 100%;

            a{
                text-decoration: none;
                color: black;
                font-weight: 500;
                transition: ease .3s;

                &:hover{
                    color: rgb(115, 0, 128);
                }
            }
        }
    }

    img{
        width: 100%;
    }
</style>