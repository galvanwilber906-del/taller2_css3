<!DOCTYPE html>
<html lang="es">
<head>

    <meta charset="UTF-8">

    <meta name="viewport" content="width=device-width, initial-scale=1.0">

    <title>Sistemas Operativos - Taller CSS3</title>

    <style>

        /* RESET */

        *{
            margin: 0;
            padding: 0;
            box-sizing: border-box;
        }


        /* BODY */

        body{
            font-family: Arial, Helvetica, sans-serif;
            background-color: #f2f2f2;
        }


        /* MENÚ FLEXBOX */

        .menu{

            display: flex;

            justify-content: center;

            gap: 20px;

            background-color: #1e1e1e;

            padding: 20px;
        }


        .menu a{

            color: white;

            text-decoration: none;

            font-size: 18px;

            transition: 0.3s;
        }


        /* HOVER MENÚ */

        .menu a:hover{

            color: cyan;
        }


        /* PRESENTACIÓN */

        .presentacion{

            text-align: center;

            padding: 40px;
        }


        .presentacion h1{

            margin-bottom: 20px;

            color: #222;
        }


        .presentacion p{

            margin-bottom: 20px;

            font-size: 18px;
        }


        /* BOTÓN */

        .boton{

            background-color: #0077ff;

            color: white;

            border: none;

            padding: 15px 25px;

            border-radius: 10px;

            cursor: pointer;

            transition: 0.3s;
        }


        /* HOVER BOTÓN */

        .boton:hover{

            background-color: green;

            transform: scale(1.1);
        }


        /* GRID */

        .galeria{

            display: grid;

            grid-template-columns: repeat(3,1fr);

            gap: 20px;

            padding: 30px;
        }


        /* CAJAS */

        .caja{

            background-color: white;

            padding: 50px;

            text-align: center;

            font-size: 20px;

            border-radius: 15px;

            transition: 0.3s;

            box-shadow: 0px 0px 10px rgba(0,0,0,0.2);
        }


        /* HOVER CAJAS */

        .caja:hover{

            background-color: #0077ff;

            color: white;

            transform: translateY(-5px);
        }


        /* RESPONSIVE DESIGN */

        @media(max-width:600px){

            .menu{

                flex-direction: column;

                align-items: center;
            }

            .galeria{

                grid-template-columns: 1fr;
            }

            .presentacion h1{

                font-size: 25px;
            }

        }

    </style>

</head>

<body>


    <!-- MENÚ FLEXBOX -->

    <header>

        <nav class="menu">

            <a href="#">Windows</a>

            <a href="#">Linux</a>

            <a href="#">MacOS</a>

            <a href="#">Android</a>

        </nav>

    </header>



    <!-- PRESENTACIÓN -->

    <section class="presentacion">

        <h1>SISTEMAS OPERATIVOS</h1>

        <p>

            Página desarrollada utilizando Flexbox,
            CSS Grid, Hover y Responsive Design
            sobre el tema de Sistemas Operativos.

        </p>

        <button class="boton">

            Ver Información

        </button>

    </section>



    <!-- GALERÍA GRID -->

    <section class="galeria">

        <div class="caja">WINDOWS</div>

        <div class="caja">LINUX</div>

        <div class="caja">MACOS</div>

        <div class="caja">ANDROID</div>

        <div class="caja">UBUNTU</div>

        <div class="caja">IOS</div>

    </section>


</body>
</html>
