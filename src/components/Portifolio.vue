<template>
    <div>
        <h1>
            <i class="fa-solid fa-list-ul" style="color: #ff5733"></i>
            Portfólio
        </h1>
        <div class="container">
            <div class="card">
                <a href="https://financeiro-empire.ddns.net/" target="_blank">
                    <img src="../assets/images/financeiro.png" class="card-img">
                </a>
                <div class="card-content">
                    <h2>Financeiro</h2>
                    <p>Financeiro é um projeto desenvolvido em Laravel, onde pode gerenciar sua vida financeira, tanto de gastos como receitas, e até para gastos e receitas fixas, e investimentos. Tem documentação, API aberta, testes unitários e muito mais.</p>
                </div>
            </div>       
        </div>
    </div>
</template>

<style scoped>
    h1 {
        margin-top: 30px;
        text-align: center;
        margin-bottom: 50px;
        color: white;
    }

    .container {
        display: flex;
        flex-wrap: wrap;
        gap: 20px;
        max-width: 1200px;
        margin: 0 auto;
        padding: 0 15px;
    }

    .card {
        flex: 1 1 calc(50% - 20px);
        box-sizing: border-box;
        background-color: #fff;
        border: 1px solid #ddd;
        border-radius: 8px;
        overflow: hidden;
        text-align: center;
        display: flex;
        flex-direction: column;
        transition: transform 0.3s ease, box-shadow 0.3s ease;
    }

    .card:hover {
        transform: scale(1.05);
        box-shadow: 0 8px 16px rgba(0, 0, 0, 0.2);
    }

    .card-img {
        width: 100%;
        height: 500px;
        object-fit: cover;
    }

    .card-content {
        padding: 20px;
        flex: 1;
    }

    .card-content h2 {
        margin: 0;
        font-size: 1.5em;
    }

    .card-content p {
        margin: 10px 0 0;
        color: #666;
    }

    @media (max-width: 900px) {
        .card {
            flex: 1 1 calc(100% - 20px); /* Ajusta para ocupar a largura total com margem */
        }

        .card-img {
            height: 400px; /* Ajusta a altura da imagem para telas menores */
        }

        .card-content h2 {
            font-size: 1.4em;
        }

        .card-content p {
            font-size: 1rem;
        }
    }

    @media (max-width: 600px) {
        .card {
            flex: 1 1 100%; /* Ocupa a largura total em telas muito pequenas */
        }

        .card-img {
            height: 300px; /* Ajusta a altura da imagem para telas pequenas */
        }

        .card-content h2 {
            font-size: 1.3em;
        }

        .card-content p {
            font-size: 0.9rem;
        }
    }
</style>
