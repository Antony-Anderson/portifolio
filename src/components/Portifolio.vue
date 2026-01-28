<template>
    <div>
        <h1>
            <i class="fa-solid fa-list-ul" style="color: #1E90FF"></i>
            Portfólio
        </h1>
        <div id="carouselPortifolio" class="carousel slide" data-bs-ride="carousel">
            <div class="carousel-inner">
                <!-- Slide 1 - Financeiro -->
                <div class="carousel-item active">
                    <div class="row">
                        <div class="col">
                            <a href="https://financeiro-empire.ddns.net/" target="_blank">
                                <img src="../assets/images/financeiro.png" class="d-block w-100" alt="Financeiro">
                            </a>
                        </div>
                        <div class="col d-flex flex-column justify-content-center">
                            <h2>Financeiro</h2>
                            <p>
                                Sistema financeiro desenvolvido com <strong>Laravel</strong> e <strong>Vue.js</strong>, 
                                contendo autenticação, controle de permissões, <strong>CRUDs</strong>, 
                                filtros por período, testes unitários e documentação da <strong>API</strong>.
                            </p>
                        </div>
                    </div>
                </div>

                <div class="carousel-item">
                    <div class="row">
                        <div class="col">
                            <a href="https://qualificabem.com/" target="_blank">
                                <img src="../assets/images/entrevista.png" class="d-block w-100" alt="Seu Projeto">
                            </a>
                        </div>
                        <div class="col d-flex flex-column justify-content-center">
                            <h2>Entrevista qualificada (trabalho atualmente)</h2>
                            <p>
                                Aplicação web desenvolvida para facilitar o gerenciamento de entrevistas e candidatos, permitindo
                                cadastro, organização e acompanhamento das informações de forma prática. O sistema foi construído
                                com <strong>Laravel</strong> seguindo o padrão <strong>MVC</strong>, utilizando <strong>API REST</strong>,
                                <strong>Eloquent ORM</strong> e banco de dados relacional, com validações e documentação das rotas.
                            </p>
                        </div>
                    </div>
                </div>
            </div>

            <button class="carousel-control-prev" type="button" data-bs-target="#carouselPortifolio" data-bs-slide="prev">
                <span class="carousel-control-prev-icon" aria-hidden="true"></span>
                <span class="visually-hidden">Previous</span>
            </button>
            <button class="carousel-control-next" type="button" data-bs-target="#carouselPortifolio" data-bs-slide="next">
                <span class="carousel-control-next-icon" aria-hidden="true"></span>
                <span class="visually-hidden">Next</span>
            </button>
        </div>
    </div>
</template>

<style scoped>
    h1 {
        color: white;
        margin-top: 30px;
        text-align: center;
        margin-bottom: 100px;
    }

    .carousel-inner {
        max-width: 1200px;
        margin: 0 auto;
        background-color: white;
        border-radius: 8px;
        overflow: hidden;
    }

    .carousel-item {
        padding: 40px;
    }

    .carousel-item .row {
        display: flex;
        align-items: center;
        gap: 40px;
    }

    .carousel-item .col:first-child {
        flex: 0 0 45%;
    }

    .carousel-item .col:last-child {
        flex: 1;
    }

    .carousel-item img {
        width: 100%;
        height: auto;
        border-radius: 8px;
        object-fit: cover;
    }

    .carousel-item h2 {
        margin: 0 0 20px 0;
        font-size: 2em;
        color: #333;
    }

    .carousel-item p {
        margin: 0;
        color: #666;
        font-size: 1.1em;
        line-height: 1.6;
    }

    .carousel-item a {
        text-decoration: none;
        display: block;
        transition: transform 0.3s ease;
    }

    .carousel-item a:hover {
        transform: scale(1.05);
    }

    .carousel-control-prev-icon {
        background-color: black;
    }

    .carousel-control-next-icon {
        background-color: black;
    }

    @media (max-width: 900px) {
        .carousel-item {
            padding: 30px;
        }

        .carousel-item .row {
            flex-direction: column;
            gap: 20px;
        }

        .carousel-item .col:first-child {
            flex: 0 0 100%;
        }

        .carousel-item h2 {
            font-size: 1.5em;
        }

        .carousel-item p {
            font-size: 1em;
        }
    }

    @media (max-width: 600px) {
        .carousel-item {
            padding: 20px;
        }

        .carousel-item h2 {
            font-size: 1.3em;
        }

        .carousel-item p {
            font-size: 0.9em;
        }
    }
</style>
