<template>
    <div class="tech-card-container">
        <h2 class="tech-title">
            <i class="fa-solid fa-laptop-code" style="color: #235ab8;"></i>
            Minhas Tecnologias
        </h2>
        <div class="tech-card">
            <div class="icons">
                <!-- Primeira linha de ícones -->
                <div class="icon-row">
                    <div class="icon-item">
                        <i class="fa-brands fa-html5" style="color: #da7210;"></i>
                        <span>HTML</span>
                    </div>
                    <div class="icon-item">
                        <i class="fa-brands fa-css3-alt" style="color: #1488e1;"></i>
                        <span>Css</span>
                    </div>
                    <div class="icon-item">
                        <i class="fa-brands fa-bootstrap" style="color: #4711e8;"></i>
                        <span>Bootstrap</span>
                    </div>
                    <div class="icon-item">
                        <i class="fa-brands fa-php" style="color: #156bb7;"></i>
                        <span>PHP</span>
                    </div>
                    <div class="icon-item">
                        <i class="fa-brands fa-laravel" style="color: #e70d11;"></i>
                        <span>Laravel</span>
                    </div>
                    <div class="icon-item">
                        <i class="fa-brands fa-js" style="color: #FFD43B;"></i>
                        <span>JavaScript</span>
                    </div>
                </div>
                <!-- Segunda linha de ícones -->
                <div class="icon-row">
                    <div class="icon-item">
                        <i class="fa-solid fa-code" style="color: #74C0FC;"></i>
                        <span>TypeScript</span>
                    </div>
                    <div class="icon-item">
                        <i class="fa-brands fa-vuejs" style="color: #63E6BE;"></i>
                        <span>Vue.js</span>
                    </div>
                    <div class="icon-item">
                        <i class="fa-brands fa-react" style="color: #74C0FC;"></i>
                        <span>React Native / React</span>
                    </div>
                    <div class="icon-item">
                        <i class="fa-solid fa-database" style="color: #b93134;"></i>
                        <span>Banco de Dados</span>
                    </div>
                </div>
            </div>
        </div>
        <h2 class="tech-title">
            <i class="fa-solid fa-font-awesome" style="color: #235ab8"></i>
            Descrição
        </h2>
        <div class="code-card">
            <pre><code>
Desenvolvimento de aplicações web robustas usando o framework Laravel, seguindo as melhores práticas de 
arquitetura MVC.
Criação e integração de APIs RESTful.
Uso avançado de Eloquent ORM para manipulação e relacionamento de dados em bancos de dados relacionais.
Implementação de testes automatizados unitários.
Gerenciamento de filas de trabalhos assíncronos usando o Laravel Queue.
Criação de documentação.

Desenvolvimento de interfaces de usuário dinâmicas e reativas utilizando Vue.js.
Criação de componentes reutilizáveis e modulares, utilizando o sistema de slots e props.
Integração de Vue Router para navegação single-page e Vuex para gerenciamento de estado global.
Uso de APIs do Vue 3, como Composition API, para um código mais modular e organizado.

Desenvolvimento de scripts front-end interativos e responsivos.
Manipulação do DOM, eventos e animações usando JavaScript puro.
Integração de bibliotecas e frameworks externos para funcionalidades adicionais, como gráficos.

Programação orientada a objetos em PHP.
Integração com sistemas de banco de dados, APIs externas e serviços web.
            </code></pre>
        </div>
    </div>
</template>

<style scoped>
    .tech-card-container {
        display: flex;
        flex-direction: column;
        justify-content: center;
        align-items: center;
        padding: 20px;
    }

    .tech-title {
        font-size: 2em;
        margin-bottom: 30px;
        text-align: center;
        color: white;
    }

    .code-card, .tech-card {
        width: 100%;
        max-width: 900px;
        padding: 20px;
        border-radius: 10px;
        box-shadow: 0 4px 12px rgba(0, 0, 0, 0.3);
        margin-bottom: 20px;
    }

    .code-card {
        background-color: #1e1e1e;
        color: #dcdcdc;
        font-family: 'Courier New', Courier, monospace;
        font-size: 1em;
        overflow-x: auto;
    }

    .tech-card {
        background-color: #f4f4f4;
        text-align: center;
    }

    .icons {
        display: flex;
        flex-direction: column;
        align-items: center;
    }

    .icon-row {
        display: flex;
        justify-content: center;
        margin-bottom: 20px;
        flex-wrap: wrap;
    }

    .icon-item {
        display: flex;
        flex-direction: column;
        align-items: center;
        margin: 15px;
        transition: transform 0.3s ease, filter 0.3s ease, opacity 0.3s ease;
    }

    .icon-item:hover {
        transform: scale(1.2);
        z-index: 1;
    }

    .icon-item:hover ~ .icon-item {
        filter: blur(2px);
        opacity: 0.5;
    }

    .icons:hover .icon-item:not(:hover) {
        filter: blur(2px);
        opacity: 0.5;
    }

    .icon-item i {
        font-size: 2.5em;
        color: #333;
    }

    .icon-item span {
        margin-top: 10px;
        font-size: 1em;
        color: #555;
    }

    @media (max-width: 768px) {
        .tech-title {
            font-size: 1.5em;
            margin-bottom: 20px;
        }

        .icon-item i {
            font-size: 2em;
        }

        .icon-item span {
            font-size: 0.9em;
        }

        .code-card, .tech-card {
            padding: 15px;
        }
    }

    @media (max-width: 480px) {
        .tech-title {
            font-size: 1.2em;
            margin-bottom: 15px;
        }

        .icon-item i {
            font-size: 1.5em;
        }

        .icon-item span {
            font-size: 0.8em;
        }

        .code-card, .tech-card {
            padding: 10px;
        }
    }
</style>
