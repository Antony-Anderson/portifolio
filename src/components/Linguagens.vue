<template>
    <div class="tech-card-container">
        <h2 class="tech-title">
            <i class="fa-solid fa-laptop-code" style="color: #1E90FF;"></i>
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
                        <i class="fa-brands fa-symfony"></i>
                        <span>Symfony</span>
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
            <i class="fa-solid fa-font-awesome" style="color: #1E90FF"></i>
            Descrição
        </h2>
        <div class="code-card">
            <pre><code>
    Desenvolvimento de aplicações web completas com foco em backend utilizando PHP (Laravel/Symfony), 
    além de interfaces modernas com Vue.js. Experiência com APIs REST, regras de negócio, 
    bancos relacionais e boas práticas de arquitetura.

    Principais competências:
    - Desenvolvimento de sistemas web utilizando Laravel seguindo arquitetura MVC
    - Criação e integração de APIs REST
    - Manipulação de dados com Eloquent ORM e relacionamentos avançados
    - Implementação de testes unitários e manutenção de qualidade do código
    - Uso de filas e jobs assíncronos com Laravel Queue
    - Criação de documentação técnica

    Front-end / Vue.js:
    - Desenvolvimento de interfaces dinâmicas com Vue 3
    - Componentização (props/slots) e reutilização de código
    - Uso de Vue Router e gerenciamento de estado (Vuex/Pinia)
    - Aplicação de Composition API para organização e escalabilidade do projeto
    
    JavaScript:
    - Criação de funcionalidades interativas, manipulação de DOM e eventos
    - Integração com bibliotecas externas (ex: gráficos, tabelas e plugins)
            </code></pre>
        </div>
        <h2 class="tech-title">
            <i class="fa-solid fa-font-awesome" style="color: #1E90FF"></i>
            Trabalho atualmente:
        </h2>
        <div class="code-card">
            <pre><code>
    Desenvolvedor Full Stack — Blue Company ({{ tempoAtuacao.anos }} {{ tempoAtuacao.anos === 1 ? 'ano' : 'anos' }} e {{ tempoAtuacao.meses }} {{ tempoAtuacao.meses === 1 ? 'mês' : 'meses' }}).
    Atuação no desenvolvimento e manutenção de aplicações web com Symfony, integrando banco de dados e APIs,
    com foco em estabilidade e evolução contínua do sistema.

    Principais atividades:

    - Desenvolvimento e manutenção de aplicações web com Symfony
    - Criação e manutenção de APIs REST
    - Implementação de CRUDs complexos com Doctrine ORM
    - Modelagem e gerenciamento de banco (MySQL/PostgreSQL)
    - Implementação de autenticação/autorização (roles/permissions/security)
    - Regras de negócio aplicando boas práticas e princípios SOLID
    - Correções, refatorações e manutenção de código legado
    - Testes automatizados e validações
    - Versionamento com Git e trabalho colaborativo com Scrum/Kanban
    - Deploy e manutenção em produção
    - Documentação técnica
            </code></pre>
        </div>
    </div>
</template>

<script setup>
    import { computed } from 'vue'
    const tempoAtuacao = computed(() => {
        const inicio = new Date(2024, 7, 25) 
        const hoje = new Date()

        let anos = hoje.getFullYear() - inicio.getFullYear()
        let meses = hoje.getMonth() - inicio.getMonth()

        if (hoje.getDate() < inicio.getDate()) {
            meses--
        }

        if (meses < 0) {
            anos--
            meses += 12
        }

        return { anos, meses }
    })
</script>


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
