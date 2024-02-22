<!DOCTYPE html>
<html lang="es">
<head>
<meta charset="UTF-8">
<meta name="viewport" content="width=device-width, initial-scale=1.0">
<title>Formulario para conocer los intereses de mi novio</title>
<style>
    body {
        font-family: Arial, sans-serif;
        background-color: #f2f2f2;
        margin: 0;
        padding: 0;
    }
    .container {
        position: relative;
        max-width: 100%;
        margin: 50px auto;
        padding: 20px;
        border-radius: 10px;
        box-shadow: 0px 0px 10px rgba(0, 0, 0, 0.1);
        overflow: hidden;
    }
    .hearts {
        position: absolute;
        top: -20px;
        left: -20px;
        right: -20px;
        bottom: -20px;
        z-index: -1;
    }
    .heart {
        position: absolute;
        width: 40px;
        height: 40px;
        background-image: url('https://emojicdn.elk.sh/❤️');
        background-size: contain;
        animation: heart-animation 1s ease infinite;
    }
    @keyframes heart-animation {
        0% { transform: scale(1); }
        50% { transform: scale(1.2); }
        100% { transform: scale(1); }
    }
    h1 {
        text-align: center;
        color: #333;
    }
    label {
        display: block;
        margin-bottom: 10px;
        color: #555;
    }
    input[type="text"],
    select {
        width: 100%;
        padding: 10px;
        margin-bottom: 20px;
        border: 1px solid #ccc;
        border-radius: 5px;
        box-sizing: border-box;
    }
    input[type="checkbox"] {
        margin-bottom: 10px;
    }
    input[type="submit"] {
        background-color: #4CAF50;
        color: white;
        padding: 15px 20px;
        border: none;
        border-radius: 5px;
        cursor: pointer;
        font-size: 16px;
        width: 100%;
    }
    input[type="submit"]:hover {
        background-color: #45a049;
    }
    #respuestas {
        margin-top: 20px;
        padding: 20px;
        border: 1px solid #ccc;
        border-radius: 5px;
        background-color: #fff;
    }
    @media only screen and (max-width: 600px) {
        .container {
            padding: 10px;
        }
        input[type="submit"] {
            font-size: 14px;
        }
    }
</style>
</head>
<body>

<div class="container">
    <h1>Formulario para conocer los intereses de mi novio</h1>
    <div class="hearts">
        <div class="heart" style="top: 20%; left: 5%;"></div>
        <div class="heart" style="top: 40%; left: 10%;"></div>
        <div class="heart" style="top: 60%; left: 20%;"></div>
        <div class="heart" style="top: 80%; left: 30%;"></div>
        <div class="heart" style="top: 10%; left: 50%;"></div>
        <div class="heart" style="top: 30%; left: 60%;"></div>
        <div class="heart" style="top: 50%; left: 70%;"></div>
        <div class="heart" style="top: 70%; left: 80%;"></div>
        <div class="heart" style="top: 90%; left: 90%;"></div>
    </div>
    <form id="formulario">
        <label for="color">¿Cuál es su color favorito?</label>
        <input type="text" id="color" name="color">

        <label for="serie">¿Cuál es su serie de televisión favorita?</label>
        <select id="serie" name="serie">
            <option value="Breaking Bad">Breaking Bad</option>
            <option value="Game of Thrones">Game of Thrones</option>
            <option value="Friends">Friends</option>
            <option value="Stranger Things">Stranger Things</option>
            <option value="The Office">The Office</option>
            <option value="Otra">Otra</option>
        </select>

        <label for="otra_serie">Si seleccionó "Otra", por favor indique cuál:</label>
        <input type="text" id="otra_serie" name="otra_serie">

        <label for="hobbies">¿Cuáles son sus pasatiempos o hobbies?</label>
        <input type="text" id="hobbies" name="hobbies">

        <label for="musica">¿Qué tipo de música prefiere?</label>
        <input type="text" id="musica" name="musica">

        <label for="pelicula">¿Cuál es su película favorita?</label>
        <input type="text" id="pelicula" name="pelicula">

        <label for="comida">¿Cuál es su comida favorita?</label>
        <input type="text" id="comida" name="comida">

        <label for="bebida">¿Cuál es su bebida favorita?</label>
        <input type="text" id="bebida" name="bebida">

        <label for="libro">¿Cuál es su libro favorito?</label>
        <input type="text" id="libro" name="libro">

        <label for="lugar">¿Cuál es su lugar favorito para pasar el tiempo libre?</label>
        <input type="text" id="lugar" name="lugar">

        <label for="videojuego">¿Cuál es su videojuego favorito?</label>
        <input type="text" id="videojuego" name="videojuego">

        <label for="instrumento">¿Toca algún instrumento musical?</label>
        <input type="text" id="instrumento" name="instrumento">
        
        <label for="superheroe">¿Cuál es su superhéroe favorito?</label>
        <input type="text" id="superheroe" name="superheroe">
        
        <label>¿Le gustan las manualidades?</label>
        <div>
            <input type="radio" id="manualidades_si" name="manualidades" value="Sí">
            <label for="manualidades_si">Sí</label>
        </div>
        <div>
            <input type="radio" id="manualidades_no" name="manualidades" value="No">
            <label for="manualidades_no">No</label>
        </div>

        <label>¿Practica algún deporte?</label>
        <div>
            <input type="checkbox" id="futbol" name="deportes" value="Fútbol">
            <label for="futbol">Fútbol</label>
        </div>
        <div>
            <input type="checkbox" id="baloncesto" name="deportes" value="Baloncesto">
            <label for="baloncesto">Baloncesto</label>
        </div>
        <div>
            <input type="checkbox" id="tenis" name="deportes" value="Tenis">
            <label for="tenis">Tenis</label>
        </div>
        <div>
            <input type="checkbox" id="otro_deporte" name="deportes" value="Otro">
            <label for="otro_deporte">Otro</label>
        </div>

        <label id="otro_deporte_label" for="otro_deporte_texto" style="display: none;">Si seleccionó "Otro", ¿cuál es su otro deporte?</label>
        <input type="text" id="otro_deporte_texto" name="otro_deporte_texto" style="display: none;">


        <input type="button" value="Enviar respuestas" onclick="mostrarRespuestas()">
    </form>

    <div id="respuestas"></div>
</div>

<script>
    function mostrarRespuestas() {
        var formulario = document.getElementById("formulario");
        var respuestasDiv = document.getElementById("respuestas");
        respuestasDiv.innerHTML = "<h2>Respuestas:</h2>";
        
        
        
        // Se muestra el valor de cada otro campo del formulario
        var otrosCampos = ["color", "serie", "otra_serie", "hobbies", "musica", "pelicula", "comida", "bebida", "libro", "lugar", "videojuego", "instrumento", "superheroe", "manualidades"];
        otrosCampos.forEach(function(campo) {
            var valorCampo = formulario.elements[campo].value.trim();
            if (valorCampo !== "") {
                respuestasDiv.innerHTML += "<p><strong>" + campo + ":</strong> " + valorCampo + "</p>";
            }
        });

        // Lógica para mostrar respuestas
        // Se muestra solo las respuestas seleccionadas en los campos de deportes
        var deportesSeleccionados = document.querySelectorAll('input[name="deportes"]:checked');
        if (deportesSeleccionados.length > 0) {
            respuestasDiv.innerHTML += "<p><strong>Deportes:</strong> ";
            deportesSeleccionados.forEach(function(deporte, index) {
                respuestasDiv.innerHTML += deporte.value;
                if (index < deportesSeleccionados.length - 1) {
                    respuestasDiv.innerHTML += ", ";
                }
            });
            respuestasDiv.innerHTML += "</p>";
        }
        
        // Se muestra el valor de "Otro deporte" si se ha seleccionado
        var otroDeporteInput = document.getElementById("otro_deporte_texto");
        if (otroDeporteInput.style.display !== "none" && otroDeporteInput.value.trim() !== "") {
            respuestasDiv.innerHTML += "<p><strong>Otro deporte:</strong> " + otroDeporteInput.value.trim() + "</p>";
        }
    }

    document.getElementById("otro_deporte").addEventListener("change", function() {
        var otroDeporteLabel = document.getElementById("otro_deporte_label");
        var otroDeporteInput = document.getElementById("otro_deporte_texto");
        if (this.checked) {
            otroDeporteLabel.style.display = "block";
            otroDeporteInput.style.display = "block";
        } else {
            otroDeporteLabel.style.display = "none";
            otroDeporteInput.style.display = "none";
            otroDeporteInput.value = ""; // Limpiar el campo si la casilla se desmarca
        }
    });
</script>



</body>
</html>







