# Formulário-Trabalho
Neste trabalho, Fiz um formulário para um site que um cliente me pediu para fazer. Ele me pediu um panfleto de sua clinica em forma digital que seria de Termo de compromisso. Que após assinar o termo de compromisso enviasse direto para o email profissional da cliente. 

<!DOCTYPE html>
<html lang="pt-br">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Documento para Preenchimento</title>
    <style>
    body {
    font-family: 'Fredoka One', cursive;
    background-color: #1d63ad; /* Um tom claro de azul como fundo */
    margin: 0;
    padding: 20px;
}

div, form {
    background-color: #fff;
    border-radius: 10px;
    padding: 20px;
    margin-bottom: 20px;
    box-shadow: 0 4px 8px rgba(0, 0, 0, 0.1);
}

label, p {
    color: #333;
    margin: 10px 0;
}

input[type="text"] {
    width: 100%;
    padding: 10px;
    margin: 5px 0 20px 0;
    border-radius: 5px;
    border: 1px solid #ccc;
    box-sizing: border-box;
}

input[type="submit"] {
    background-color: #007bff; /* Um azul mais vibrante para o botão */
    color: white;
    padding: 12px 20px;
    border: none;
    border-radius: 5px;
    cursor: pointer;
    transition: background-color 0.3s ease;
}

input[type="submit"]:hover {
    background-color: #0056b3; /* Um tom de azul mais escuro ao passar o mouse */
}

hr {
    border-top: 1px solid #ccc;
    margin-top: 20px;
    margin-bottom: 20px;
}


        </style>
        
    <link href="https://fonts.googleapis.com/css2?family=Fredoka+One&display=swap" rel="stylesheet">

</head>
<body>
<form action="https://formspree.io/f/xbjnglna" method="POST">
        <div>
            <p>1- Não será realizado o evento para crianças sem autorização.</p>
            <p>2- Alteração da data do evento deverá ser informada com 
                <input type="text" id="dias-antecedencia" name="dias_antecedencia" required> dias de antecedência mediante a consulta.</p>
        </div>
        
        <label for="evento-sem1">1º SEM - O evento será realizado nos dias:</label>
        <input type="text" id="evento-sem1" name="evento_sem1" required><br>e no período de 
        <input type="text" id="periodo-sem1" name="periodo_sem1" required>
        
        <p>As fichas de autorização e o valor acordado serão recolhidos em 
            <input type="text" id="recolhimento-sem1" name="recolhimento_sem1" required> 
            <br> A não entrega no dia estipulado acarretará em novo agendamento.</p>
        
        <hr>
        
        <label for="evento-sem2">2º SEM - O evento será realizado nos dias:</label>
        <input type="text" id="evento-sem2" name="evento_sem2" required>
        <br> e no período de 
        <input type="text" id="periodo-sem2" name="periodo_sem2" required>
        
        <p>As fichas de autorização e o valor acordado serão recolhidos em 
            <input type="text" id="recolhimento-sem2" name="recolhimento_sem2" required> 
             A não entrega no dia estipulado acarretará em novo agendamento.</p>

        <input type="submit" value="Enviar">
    </form>
    
    <script>
        window.onload = function() {
            document.querySelector('form').onsubmit = function(e) {
                // A lógica de validação permanece a mesma
            };
        };
    </script>
</body>
</html>
