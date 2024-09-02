<!DOCTYPE html>
<html lang="es">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Comprar Auriculares</title>
    <style>
        body {
            font-family: Arial, sans-serif;
            display: flex;
            justify-content: center;
            padding: 20px;
            background-color: #f7f7f7;
        }
        .container {
            display: flex;
            max-width: 1200px;
            width: 100%;
            flex-wrap: wrap;
        }
        .left-column, .right-column {
            padding: 20px;
            background-color: #fff;
            border-radius: 10px;
            box-shadow: 0 0 10px rgba(0, 0, 0, 0.1);
            margin: 10px;
        }
        .left-column {
            flex: 2;
        }
        .right-column {
            flex: 1;
            text-align: center;
        }
        .product-container {
            display: none;
        }
        .product-container img {
            width: 300px; /* Establece un tamaño fijo para todas las imágenes */
            height: 300px; /* Ajusta la altura para que sea uniforme */
            object-fit: cover; /* Mantiene la proporción y recorta las imágenes si es necesario */
            border-radius: 10px;
            margin-top: 10px;
        }
        .product-container h2 {
            color: #333;
            font-size: 20px;
            margin-top: 10px;
        }
        .product-container p {
            color: #666;
            font-size: 16px;
        }
        .product-container form {
            margin-top: 10px;
        }
        button {
            margin-top: 10px;
            padding: 10px 20px;
            background-color: #ff9900;
            color: white;
            border: none;
            border-radius: 5px;
            cursor: pointer;
            font-size: 16px;
        }
        button:hover {
            background-color: #e68a00;
        }
        video {
            width: 100%; /* Asegura que el video ocupe todo el ancho de la columna */
            height: auto;
            border-radius: 10px;
        }
    </style>
</head>
<body>
    <div class="container">
        <!-- Columna izquierda: Selección de productos -->
        <div class="left-column">
            <h1>Selecciona la Marca de Auriculares</h1>
            
            <!-- Selección de marca -->
            <div class="brand-selection">
                <label for="marca">Elige una marca:</label>
                <select id="marca" onchange="mostrarProductos()">
                    <option value="">--Selecciona una marca--</option>
                    <option value="marca1">Marca 1</option>
                    <option value="marca2">Marca 2</option>
                </select>
            </div>

            <!-- Productos de Marca 1 -->
            <div id="productos-marca1" class="product-container">
                <h2>Auriculares Marca 1 - Modelo 1</h2>
                <img src="https://http2.mlstatic.com/D_NQ_NP_938530-MLU70651258877_072023-O.webp" alt="Auriculares Marca 1 - Modelo 1">
                <p>Auriculares de alta calidad, modelo 1 de la Marca 1. Precio: $60.00</p>
                <form action="https://www.paypal.com/cgi-bin/webscr" method="post" target="_top">
                    <input type="hidden" name="cmd" value="_xclick">
                    <input type="hidden" name="business" value="TU_CORREO_PAYPAL@ejemplo.com">
                    <input type="hidden" name="item_name" value="Auriculares Marca 1 - Modelo 1">
                    <input type="hidden" name="amount" value="60.00">
                    <input type="hidden" name="currency_code" value="USD">
                    <input type="submit" value="Comprar ahora con PayPal">
                </form>

                <h2>Auriculares Marca 1 - Modelo 2</h2>
                <img src="https://http2.mlstatic.com/D_NQ_NP_938530-MLU70651258877_072023-O.webp" alt="Auriculares Marca 1 - Modelo 2">
                <p>Auriculares de alta calidad, modelo 2 de la Marca 1. Precio: $70.00</p>
                <form action="https://www.paypal.com/cgi-bin/webscr" method="post" target="_top">
                    <input type="hidden" name="cmd" value="_xclick">
                    <input type="hidden" name="business" value="TU_CORREO_PAYPAL@ejemplo.com">
                    <input type="hidden" name="item_name" value="Auriculares Marca 1 - Modelo 2">
                    <input type="hidden" name="amount" value="70.00">
                    <input type="hidden" name="currency_code" value="USD">
                    <input type="submit" value="Comprar ahora con PayPal">
                </form>
            </div>

            <!-- Productos de Marca 2 -->
            <div id="productos-marca2" class="product-container">
                <h2>Auriculares Marca 2 - Modelo 1</h2>
                <img src="https://http2.mlstatic.com/D_NQ_NP_938530-MLU70651258877_072023-O.webp" alt="Auriculares Marca 2 - Modelo 1">
                <p>Auriculares de alta calidad, modelo 1 de la Marca 2. Precio: $65.00</p>
                <form action="https://www.paypal.com/cgi-bin/webscr" method="post" target="_top">
                    <input type="hidden" name="cmd" value="_xclick">
                    <input type="hidden" name="business" value="TU_CORREO_PAYPAL@ejemplo.com">
                    <input type="hidden" name="item_name" value="Auriculares Marca 2 - Modelo 1">
                    <input type="hidden" name="amount" value="65.00">
                    <input type="hidden" name="currency_code" value="USD">
                    <input type="submit" value="Comprar ahora con PayPal">
                </form>

                <h2>Auriculares Marca 2 - Modelo 2</h2>
                <img src="https://http2.mlstatic.com/D_NQ_NP_938530-MLU70651258877_072023-O.webp" alt="Auriculares Marca 2 - Modelo 2">
                <p>Auriculares de alta calidad, modelo 2 de la Marca 2. Precio: $75.00</p>
                <form action="https://www.paypal.com/cgi-bin/webscr" method="post" target="_top">
                    <input type="hidden" name="cmd" value="_xclick">
                    <input type="hidden" name="business" value="TU_CORREO_PAYPAL@ejemplo.com">
                    <input type="hidden" name="item_name" value="Auriculares Marca 2 - Modelo 2">
                    <input type="hidden" name="amount" value="75.00">
                    <input type="hidden" name="currency_code" value="USD">
                    <input type="submit" value="Comprar ahora con PayPal">
                </form>
            </div>
        </div>

        <!-- Columna derecha: Video de publicidad -->
        <div class="right-column">
            <h2>Publicidad Auriculares Xiaomi</h2>
            <video controls>
                <source src="C:/Users/Gerardo Curia/Downloads/Redmi Airdots 2 Official Video.mp4" type="video/mp4">
                Tu navegador no soporta la reproducción de videos.
            </video>
        </div>
    </div>

    <script>
        function mostrarProductos() {
            // Ocultar todos los productos
            document.getElementById('productos-marca1').style.display = 'none';
            document.getElementById('productos-marca2').style.display = 'none';
            
            // Mostrar los productos según la marca seleccionada
            var marcaSeleccionada = document.getElementById('marca').value;
            if (marcaSeleccionada === 'marca1') {
                document.getElementById('productos-marca1').style.display = 'block';
            } else if (marcaSeleccionada === 'marca2') {
                document.getElementById('productos-marca2').style.display = 'block';
            }
        }
    </script>
</body>
</html>
