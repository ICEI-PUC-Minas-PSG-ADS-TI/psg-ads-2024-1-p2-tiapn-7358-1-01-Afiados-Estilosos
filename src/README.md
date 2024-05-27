# Código-fonte do projeto
HTML da tela de Serviços:

<!DOCTYPE html>
<html lang="en">

<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Serviços Barbearia</title>
    <link rel="stylesheet" href="serviços.css">
</head>

<body>
    <header>
        
        <nav class="menu-desktop">
            <ul>
                <li><a href="#">Inicio</a></li>
                <li><a href="#">Serviço</a></li>
                <li><a href="#">Agendamento</a></li>
                <li><a href="#">Contato</a></li>
            </ul>
        </nav>

        <div class="btn-perfil">
            <a href="#">
                <button>Perfil</button>
            </a>
        </div>
        </div>
    </header>

    <main>
        <h1>Confira nossos serviços!</h1>
        <div class="tela">
            <div class="corte">
                <h2 class="titulo-corte">Corte</h2>
                    <h3>Cabelo - R$35,00</h3>
                    <h3>Barba - R$25,00</h3>
                    <h3>Cabelo e Barba - R$60,00</h3>
                    <h3>Sobrancelha- R$13,00</h3>
                    <h3>Pézinho - R$15,00</h3>
            </div>

            <div class="hidratacao">
                <h2 class="titulo-hidratacao">Hidratação e Química
                    <h3>Limpeza de pele - R$20,00</h3>
                    <h3>Hidratação capilar - R$20,00</h3>
                    <h3>Relaxamento - R$25,00</h3>
                    <h3>Pigmentação - R$25,00</h3>
                    <h3>Platinado/Luzes - R$120,00</h3>
                </h2>
            </div>
        </div>
    </main>

    <footer>
        <div class="rodape">
            <h4>
                Copyright (c) Afiados & Estilosos - 2024
            </h4>
        </div>
    </footer>
    
</body>
</html>

CSS da tela de Serviços:

/*ESTILO EM GERAL*/
*{
    margin: 0;
    padding: 0;
    box-sizing: border-box;
}

body{
    background-color: rgb(33, 0, 63);
    height: 100ch;
}

.interface{
    max-width: 1280px;
    margin: 0 auto;
}

/*ESTILO CABECALHO*/
header{
    padding: 40px 4%;
    display: flex;
    align-items: center;
    justify-content: center;
    font-family: Arial, Helvetica, sans-serif;
    font-size: 18px;
}

header a{
    color: rgb(255, 255, 255);
    text-decoration: none;
    display: inline-block;
    transition: 0.5s;

}

header a:hover{
    color: rgb(255, 255, 0);
    transform: scale(1.30);

}

header nav ul{
    list-style-type: none;
}

header nav ul li{
    display: inline-block;
    padding: 0 45px;
}

header .btn-perfil button{
    padding: 20px 40px;
    font-size: 22px;
    font-weight: 700;
    border: 0;
    border-radius: 30px;
    cursor: pointer;
}

header .btn-perfil button:hover{
    box-shadow: 0px 0px 8px #ffd000;

}

main{
    font-family: Arial, Helvetica, sans-serif;
    margin-top: 30px;
}

main h1{
    text-align: center;
    font-size: 60px;
    padding: 30px;
    color: white;
    font-weight: 800;

}

.tela{
    display: flex;
    justify-content: center;
    background-color: white;
    margin-left: 450px;
    width: 1000px;
    height: 300px;
    border-top-left-radius: 10px; 
    border-top-right-radius: 10px; 
    border-bottom-left-radius: 10px;
    border-bottom-right-radius: 10px;
}



.corte{
    font-size: 20px;
    float: left;
    margin-left: 20px;
    margin-right: 16%;
    margin-top: 40px;
}

.hidratacao{
    font-size: 20px;
    margin-top: 40px;
}

.titulo-corte{
    text-align: center;
    font-size: 30px;
    background-color: rgb(59, 0, 114);
    color: white;
    border-radius: 5px;
}

.titulo-hidratacao{
    text-align: center;
    font-size: 30px;
    background-color: rgb(59, 0, 114);
    color: white;
    border-radius: 5px;
}
main h3{
    margin-top: 6px;
}
main h2{
    margin-bottom: 20px;
}

/*Estilização do footer*/
footer{
    position: fixed;
    bottom: 0;
    padding: 20px;
    width: 100%;
    color: antiquewhite;
    background-color: rgba(49, 0, 174, 0.837);
    padding: 15px;
    text-align: center;
    font-family: Arial, Helvetica, sans-serif;
    ;
}

.footer-section {
    flex: 1 1 200px;
    margin: 10px;
    padding: 10px;
    box-sizing: border-box;
  }

  .footer-section h3 {
    margin-top: 0;
  }

  .footer-section ul {
    list-style: none;
    padding: 0;
  }

  .footer-section ul li {
    margin: 5px 0;
  }

  .footer-section ul li a {
    color: white;
    text-decoration: none;
  }

  .footer-section ul li a:hover {
    text-decoration: underline;
  }

  @media (max-width: 600px) {
    .container {
      flex-direction: column;
      align-items: center;
    }
}

