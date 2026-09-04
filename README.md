<!DOCTYPE html>
<html lang="es">

<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">

    <title>Para Dayanna ❤️</title>

    <style>

        /* =========================
           CONFIGURACIÓN GENERAL
        ========================= */

        * {
            box-sizing: border-box;
        }

        html,
        body {
            width: 100%;
            min-height: 100%;
            margin: 0;
        }

        body {
            min-height: 100vh;

            display: flex;
            justify-content: center;
            align-items: center;

            padding: 20px;

            font-family: Arial, sans-serif;

            background:
                radial-gradient(circle at top left,
                    rgba(255, 255, 255, 0.25),
                    transparent 35%),
                linear-gradient(
                    135deg,
                    #ff758c,
                    #ff7eb3,
                    #ff9a9e
                );

            overflow: hidden;
        }


        /* =========================
           CORAZONES DEL FONDO
        ========================= */

        .corazon-fondo {
            position: fixed;

            bottom: -50px;

            color: rgba(255, 255, 255, 0.35);

            font-size: 20px;

            pointer-events: none;

            animation: flotar linear infinite;

            z-index: 0;
        }

        @keyframes flotar {

            0% {
                transform:
                    translateY(0)
                    rotate(0deg);

                opacity: 0;
            }

            15% {
                opacity: 1;
            }

            100% {
                transform:
                    translateY(-120vh)
                    rotate(360deg);

                opacity: 0;
            }
        }


        /* =========================
           PANTALLAS
        ========================= */

        .pantalla {

            width: 100%;
            max-width: 550px;

            padding: 45px 30px;

            background: rgba(255, 255, 255, 0.96);

            border-radius: 30px;

            text-align: center;

            box-shadow:
                0 15px 50px rgba(0, 0, 0, 0.25);

            position: relative;

            z-index: 2;

            animation: aparecer 0.8s ease;

            backdrop-filter: blur(5px);
        }


        .oculta {
            display: none;
        }


        @keyframes aparecer {

            from {
                opacity: 0;
                transform: scale(0.75) translateY(20px);
            }

            to {
                opacity: 1;
                transform: scale(1) translateY(0);
            }

        }


        /* =========================
           PANTALLA 1
        ========================= */

        #pantalla1 h1 {

            color: #ff3366;

            font-size: 38px;

            margin: 0 0 20px;

            animation: latido 1.5s infinite;
        }


        @keyframes latido {

            0%,
            100% {
                transform: scale(1);
            }

            50% {
                transform: scale(1.05);
            }
        }


        #pantalla1 p {

            color: #555;

            font-size: 20px;

            line-height: 1.5;

            margin: 10px 0;
        }


        .pregunta {

            font-size: 29px;

            font-weight: bold;

            color: #333;

            margin: 30px 0;

            line-height: 1.3;
        }


        /* =========================
           BOTONES
        ========================= */

        .botones {

            display: flex;

            justify-content: center;

            align-items: center;

            flex-wrap: wrap;

            min-height: 80px;

            position: relative;
        }


        button {

            border: none;

            padding: 15px 28px;

            border-radius: 30px;

            font-size: 18px;

            font-weight: bold;

            cursor: pointer;

            margin: 10px;

            transition:
                transform 0.2s ease,
                box-shadow 0.2s ease;

            -webkit-tap-highlight-color: transparent;
        }


        #si {

            background:
                linear-gradient(
                    135deg,
                    #ff3366,
                    #ff174f
                );

            color: white;

            box-shadow:
                0 7px 20px rgba(255, 51, 102, 0.35);
        }


        #si:hover {

            transform: scale(1.1);

            box-shadow:
                0 10px 25px rgba(255, 51, 102, 0.5);
        }


        #si:active {

            transform: scale(0.95);
        }


        #no {

            background: #555;

            color: white;

            box-shadow:
                0 5px 15px rgba(0, 0, 0, 0.2);

            position: relative;
        }


        /* =========================
           PANTALLA 2
        ========================= */

        #pantalla2 {

            padding-top: 40px;
            padding-bottom: 40px;
        }


        #pantalla2 h1 {

            color: #ff3366;

            font-size: 35px;

            margin: 0 0 25px;

            line-height: 1.25;
        }


        #pantalla2 p {

            color: #ff3366;

            font-size: 21px;

            font-weight: bold;

            line-height: 1.6;

            margin: 22px 0;
        }


        .decoracion {

            font-size: 35px;

            margin-bottom: 15px;

            animation: latido 1.5s infinite;
        }


        .firma {

            color: #ff3366;

            font-size: 23px;

            font-weight: bold;

            margin-top: 30px;

            line-height: 1.5;
        }


        .captura {

            display: inline-block;

            margin-top: 10px;

            padding: 10px 18px;

            border-radius: 20px;

            background: #fff0f4;

            color: #ff3366;

            font-size: 18px;
        }


        /* =========================
           CORAZONES AL ACEPTAR
        ========================= */

        .corazon {

            position: fixed;

            top: -50px;

            font-size: 25px;

            animation: caer linear forwards;

            z-index: 10;

            pointer-events: none;
        }


        @keyframes caer {

            0% {

                transform:
                    translateY(-50px)
                    rotate(0deg)
                    scale(1);

                opacity: 1;
            }

            50% {

                opacity: 1;
            }

            100% {

                transform:
                    translateY(110vh)
                    rotate(360deg)
                    scale(1.2);

                opacity: 0;
            }

        }


        /* =========================
           RESPONSIVE - CELULAR
        ========================= */

        @media (max-width: 600px) {

            body {
                padding: 15px;
            }


            .pantalla {

                width: 100%;

                padding: 35px 20px;

                border-radius: 25px;
            }


            #pantalla1 h1 {

                font-size: 30px;

                margin-bottom: 15px;
            }


            #pantalla1 p {

                font-size: 18px;
            }


            .pregunta {

                font-size: 24px;

                margin: 25px 0;
            }


            button {

                padding: 14px 22px;

                font-size: 16px;
            }


            #pantalla2 h1 {

                font-size: 28px;
            }


            #pantalla2 p {

                font-size: 18px;

                line-height: 1.5;
            }


            .firma {

                font-size: 20px;
            }


            .captura {

                font-size: 16px;
            }
        }


        /* =========================
           CELULARES PEQUEÑOS
        ========================= */

        @media (max-width: 380px) {

            .pantalla {

                padding: 30px 16px;
            }


            #pantalla1 h1 {

                font-size: 27px;
            }


            .pregunta {

                font-size: 22px;
            }


            button {

                padding: 13px 18px;

                font-size: 15px;
            }
        }

    </style>

</head>


<body>


    <!-- =========================
         CORAZONES DEL FONDO
    ========================= -->

    <div class="corazon-fondo" style="left: 5%; animation-duration: 9s;">
        ❤️
    </div>

    <div class="corazon-fondo" style="left: 18%; animation-duration: 12s;">
        💕
    </div>

    <div class="corazon-fondo" style="left: 32%; animation-duration: 10s;">
        ❤️
    </div>

    <div class="corazon-fondo" style="left: 48%; animation-duration: 14s;">
        💗
    </div>

    <div class="corazon-fondo" style="left: 63%; animation-duration: 11s;">
        ❤️
    </div>

    <div class="corazon-fondo" style="left: 78%; animation-duration: 13s;">
        💕
    </div>

    <div class="corazon-fondo" style="left: 92%; animation-duration: 10s;">
        ❤️
    </div>


    <!-- =========================
         PANTALLA 1
    ========================= -->

    <div id="pantalla1" class="pantalla">

        <h1>
            💕 Hola, mi niña 💕
        </h1>


        <p>
            Tengo una pregunta muy importante
            para ti... ❤️
        </p>


        <div class="pregunta">

            ¿Quieres formar parte de mi vida? 🥰❤️

        </div>


        <div class="botones">

            <button id="si" onclick="aceptar()">

                ❤️ SÍ, QUIERO

            </button>


            <button id="no">

                😏 NO

            </button>

        </div>

    </div>


    <!-- =========================
         PANTALLA 2
    ========================= -->

    <div id="pantalla2" class="pantalla oculta">

        <div class="decoracion">
            💕❤️💕
        </div>


        <h1>

            💕 ¡Sabía que dirías que sí! 💕

        </h1>


        <p>

            Dayanna, quiero compartir contigo
            momentos lindos, crear recuerdos
            que nunca olvidemos y vivir una
            historia juntos. 🥰❤️

        </p>


        <p>

            Quiero estar a tu lado, reír contigo,
            apoyarte y disfrutar cada momento
            que la vida nos regale. 💕

        </p>


        <div class="firma">

            ❤️ Con cariño, David ❤️

            <br>

            <span class="captura">
                📸 Me envías una captura
            </span>

        </div>

    </div>


    <script>


        /* =========================
           BOTÓN NO
        ========================= */

        const botonNo =
            document.getElementById("no");


        botonNo.addEventListener(
            "mouseenter",
            escapar
        );


        botonNo.addEventListener(
            "touchstart",
            escapar,
            {
                passive: true
            }
        );


        function escapar() {

            const margen = 15;


            const anchoMaximo =
                window.innerWidth -
                botonNo.offsetWidth -
                margen;


            const altoMaximo =
                window.innerHeight -
                botonNo.offsetHeight -
                margen;


            const x =
                Math.max(
                    margen,
                    Math.random() * anchoMaximo
                );


            const y =
                Math.max(
                    margen,
                    Math.random() * altoMaximo
                );


            botonNo.style.position =
                "fixed";


            botonNo.style.left =
                x + "px";


            botonNo.style.top =
                y + "px";

        }


        /* =========================
           BOTÓN SÍ
        ========================= */

        function aceptar() {

            const pantalla1 =
                document.getElementById(
                    "pantalla1"
                );


            const pantalla2 =
                document.getElementById(
                    "pantalla2"
                );


            /* Ocultar pantalla 1 */

            pantalla1.classList.add(
                "oculta"
            );


            /* Mostrar pantalla 2 */

            pantalla2.classList.remove(
                "oculta"
            );


            /* Crear lluvia de corazones */

            crearCorazones();

        }


        /* =========================
           CREAR CORAZONES
        ========================= */

        function crearCorazones() {

            for (
                let i = 0;
                i < 60;
                i++
            ) {

                const corazon =
                    document.createElement(
                        "div"
                    );


                corazon.classList.add(
                    "corazon"
                );


                corazon.innerHTML =
                    Math.random() > 0.5
                        ? "❤️"
                        : "💕";


                corazon.style.left =
                    Math.random() * 100 +
                    "vw";


                corazon.style.animationDuration =
                    (Math.random() * 4 + 3) +
                    "s";


                corazon.style.fontSize =
                    (Math.random() * 25 + 15) +
                    "px";


                document.body.appendChild(
                    corazon
                );


                setTimeout(() => {

                    corazon.remove();

                }, 8000);

            }

        }


    </script>


</body>

</html>
