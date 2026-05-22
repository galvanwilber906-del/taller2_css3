<!DOCTYPE html>
<html lang="es">
<head>

    <meta charset="UTF-8">

    <meta name="viewport" content="width=device-width, initial-scale=1.0">

    <title>Taller CSS3</title>

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

            background-color: #222;

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

            color: yellow;
        }


        /* PRESENTACIÓN */

        .presentacion{

            text-align: center;

            padding: 40px;
        }


        .presentacion h1{

            margin-bottom: 20px;

            color: #333;
        }


        .presentacion p{

            margin-bottom: 20px;

            font-size: 18px;
        }


        /* BOTÓN */

        .boton{

            background-color: blue;

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

            background-color: lightgray;

            padding: 60px;

            text-align: center;

            font-size: 20px;

            border-radius: 15px;

            transition: 0.3s;
        }


        /* HOVER CAJAS */

        .caja:hover{

            background-color: orange;

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

            <a href="#">Inicio</a>

            <a href="#">Noticias</a>

            <a href="#">Galería</a>

            <a href="#">Contacto</a>

        </nav>

    </header>



    <!-- PRESENTACIÓN -->

    <section class="presentacion">

        <h1>TECNOLOGÍA Y DESARROLLO WEB</h1>

        <p>

            Página creada utilizando Flexbox, CSS Grid,
            Hover y Responsive Design.

        </p>

        <button class="boton">

            Más Información

        </button>

    </section>



    <!-- GALERÍA GRID -->

    <section class="galeria">

        <div class="caja">HTML5</div>

        <div class="caja">CSS3</div>

        <div class="caja">JAVASCRIPT</div>

        <div class="caja">FLEXBOX</div>

        <div class="caja">GRID</div>

        <div class="caja">RESPONSIVE</div>

    </section>


</body>
</html>
