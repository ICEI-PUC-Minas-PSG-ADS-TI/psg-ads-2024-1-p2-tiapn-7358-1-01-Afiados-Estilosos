
Tela Home Page
<!DOCTYPE html>
<html lang="pt-br">

<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=
   , initial-scale=1.0">
    <title>Home</title>
    <link rel="stylesheet" href="cssHome.css">



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
        </div><!--inetface-->
    </header>

    <main>
        <section class="topo-site">
            <div class="interface">
                <div class="flex">
                    <div class="img-topo-site">
                        <img src="imgHome/img-home-afiados-estilosos.png" alt="">
                    </div>
                </div>
            </div><!--fim interface-->
        </section><!--fim topo site-->

        <section class="meio-site">
            <div class="flex2">
                <h1>DIVERSOS SERVIÇOS</h1>

                <div class="display-img">
                    <div class="imgbarba">
                        <img src="imgHome/img-Home-BARBA.jpg" alt="">
                        <h2>BARBA</h2>
                    </div>

                    <div class="imgcorte">
                        <img src="imgHome/img-Home-CORTE.jpg" alt="">
                        <h2>CORTES</h2>
                    </div>

                    <div class="imgpigmentacao">
                        <img src="imgHome/img-Home-PIGMENTAÇÃO.jpg" alt="">
                        <h2>PIGMENTAÇÕES</h2>
                    </div>
                </div>
            </div>
            </div>
        </section>
    </main>

    <footer>
        <div class="rodape">
            <h4>Copyright (c) Afiados & Estilosos - 2024 </h4>
        </div>
    </footer>

</body>

</html>


#css Home Page 

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

/*ESTILO TOPO IMG*/

section.topo-site{
    padding: 10px 4%;
}

.flex{
    display: flex;
    
}

section.topo-site .flex{
    align-items: center;
    justify-content: center;
}


/*ESTILO MEIO SITE IMG*/


.flex2 h1{
    text-align: center;
    padding: 5px;
    margin: 50px;
    color: rgb(255, 255, 255);
    font-family: Arial, Helvetica, sans-serif;
 
}

.flex2 h2{
    color: aliceblue;
    justify-content: left;
    font-family: Arial, Helvetica, sans-serif ;
    text-align: center;
    
}

.display-img{
    display: flex;
    max-width: 100%;
    height: auto;
    
}

section.meio-site .display-img{
      align-items: center;
      justify-content: center;
      padding: 15px;
      gap: 100px;  
      
}

.display-img{
    width: 100%;
    height: 100%;
    
}


footer{
    width: 100%;
    color: antiquewhite;
    background-color: rgba(49, 0, 174, 0.837);
    padding: 15px;
    text-align: center;
    font-family: Arial, Helvetica, sans-serif;
   
}


*Imagens Home Page 


![img-Home-BARBA](https://github.com/ICEI-PUC-Minas-PSG-ADS-TI/psg-ads-2024-1-p2-tiapn-7358-1-01-Afiados-Estilosos/assets/129122228/f1ee77fb-afba-4322-af65-312627bc4e6c)
![img-home-afiados-estilosos](https://github.com/ICEI-PUC-Minas-PSG-ADS-TI/psg-ads-2024-1-p2-tiapn-7358-1-01-Afiados-Estilosos/assets/129122228/bf8f6bad-2188-49f3-b1a9-0ed72ea2f583)
![img-Home-PIGMENTAÇÃO](https://github.com/ICEI-PUC-Minas-PSG-ADS-TI/psg-ads-2024-1-p2-tiapn-7358-1-01-Afiados-Estilosos/assets/129122228/6ac7b4b3-718f-47bb-919f-79e11e0a940d)
![img-Home-CORTE](https://github.com/ICEI-PUC-Minas-PSG-ADS-TI/psg-ads-2024-1-p2-tiapn-7358-1-01-Afiados-Estilosos/assets/129122228/9bb7f8bd-1786-4911-bab7-3fb283f28bae)




