<template>
    <div>
        <head>
            <meta charset="UTF-8">
            <meta name="viewport" content="width=device-width, initial-scale=1.0">
            <title>Card Exemplo</title>
            <link rel="stylesheet" href="styles.css">
        </head>
        <body>
            <div class="card-container">
                <div class="card">
                    <h1 class="card-title">Título do Card</h1>
                    <p class="card-description">Esta é a descrição do card. Aqui você pode adicionar mais detalhes sobre o conteúdo deste card.</p>
                </div>
            </div>
        </body>
    </div>
</template>

<style scoped>
    h1{
        margin-top: 30px;
        text-align: center;
    }
    body, html {
        text-shadow: 2px 2px 4px rgba(0, 0, 0, 0.5);
        margin: 0;
        padding: 0;
        height: 100%;
        display: flex;
        justify-content: center;
        align-items: center;
        background-color: #f0f0f0;
        font-family: Arial, sans-serif;
    }

    .card-container {
        width: 100%;
        height: 100%;
        display: flex;
        justify-content: center;
        align-items: center;
    }

    .card {
        background-color: #ffffff;
        border-radius: 10px;
        box-shadow: 0 4px 8px rgba(0, 0, 0, 0.1);
        padding: 40px;
        max-width: 80%;
        text-align: center;
        transform: scale(0.8);
        animation: grow 1s ease-out forwards;
        transition: transform 0.3s ease, box-shadow 0.3s ease;
    }

    .card-title {
        font-size: 2.5rem;
        margin-bottom: 20px;
    }

    .card-description {
        font-size: 1.2rem;
        color: #555555;
    }

    .card:hover {
        transform: scale(1.05);
        box-shadow: 0 8px 16px rgba(0, 0, 0, 0.2);
    }

    @keyframes grow {
        0% {
            transform: scale(0.8);
            background-color: #e0e0e0;
        }
        100% {
            transform: scale(1);
            background-color: #ffffff;
        }
    }
</style>