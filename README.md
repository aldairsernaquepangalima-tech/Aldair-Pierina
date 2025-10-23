
<!DOCTYPE html>
<html lang="es">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Sube tu Foto</title>
    <style>
        body {
            font-family: Arial, sans-serif;
            display: flex;
            justify-content: center;
            align-items: center;
            min-height: 100vh;
            margin: 0;
            background-color: #f4f4f9;
        }
        .container {
            background-color: #fff;
            padding: 30px;
            border-radius: 8px;
            box-shadow: 0 4px 8px rgba(0, 0, 0, 0.1);
            text-align: center;
        }
        h1 {
            color: #333;
            margin-bottom: 20px;
        }
        .upload-form {
            display: flex;
            flex-direction: column;
            gap: 15px;
        }
        .upload-form input[type="file"] {
            padding: 10px;
            border: 1px solid #ccc;
            border-radius: 4px;
        }
        .upload-form button {
            background-color: #007bff;
            color: white;
            padding: 10px 15px;
            border: none;
            border-radius: 4px;
            cursor: pointer;
            font-size: 16px;
            transition: background-color 0.3s;
        }
        .upload-form button:hover {
            background-color: #0056b3;
        }
    </style>
</head>
<body>

<div class="container">
    <h1>🖼️ Sube tu Foto</h1>

    <form action="upload.php" method="POST" enctype="multipart/form-data" class="upload-form">
        
        <label for="photo-file">Selecciona una imagen:</label>
        
        <input type="file" id="photo-file" name="image_file" accept="image/*" required>

        <button type="submit">Subir Foto</button>
    </form>
    
    <p>La subida real requiere un script de servidor.</p>
</div>

</body>
</html>
