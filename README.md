
<html lang="es">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Móvil Express - Oficial</title>
    <style>
        :root {
            --azul: #003366;
            --rojo: #d32f2f;
            --amarillo: #ffcc00;
        }
        body {
            font-family: sans-serif;
            margin: 0;
            background-color: var(--azul);
            color: white;
            text-align: center;
        }
        .header {
            background: linear-gradient(135deg, var(--rojo), #ff8800);
            padding: 25px;
            font-weight: bold;
        }
        .container {
            padding: 20px;
            max-width: 450px;
            margin: auto;
        }
        .servicio {
            background: white;
            color: #333;
            margin: 10px 0;
            padding: 15px;
            border-radius: 10px;
            border-left: 10px solid var(--rojo);
            text-align: left;
            font-weight: bold;
        }
        input, textarea {
            width: 100%;
            padding: 12px;
            margin: 10px 0;
            border-radius: 5px;
            border: none;
            box-sizing: border-box;
        }
        button {
            background: var(--amarillo);
            color: #000;
            width: 100%;
            padding: 15px;
            border: none;
            border-radius: 10px;
            font-weight: bold;
            font-size: 1.1rem;
            cursor: pointer;
        }
    </style>
</head>
<body>
    <div class="header">
        <h1 style="margin:0;">MÓVIL EXPRESS</h1>
        <p style="margin:5px 0 0 0;">VENTA Y ACTIVACIÓN</p>
    </div>

    <div class="container">
        <div class="servicio">✅ Venta y Activación de eSIM</div>
        <div class="servicio">✅ Liberaciones y Desbloqueos</div>
        <div class="servicio">✅ Cuenta Google e iCloud</div>
        <div class="servicio">✅ Cambio de Display</div>

        <form id="wa">
            <input type="text" id="n" placeholder="Tu nombre" required>
            <textarea id="s" placeholder="¿Qué servicio necesitas?" rows="3" required></textarea>
            <button type="submit">PEDIR POR WHATSAPP</button>
        </form>
    </div>

    <script>
        document.getElementById('wa').onsubmit = function(e) {
            e.preventDefault();
            const n = document.getElementById('n').value;
            const s = document.getElementById('s').value;
            window.open(`https://wa.me/+522203509986?text=Móvil%20Express%0ACliente:%20${n}%0AServicio:%20${s}`);
        };
    </script>
</body>
</html>
