#<h2> BIBLIOTEC</h2>

Integrantes: Bianca e Leonardo Agripino<br>
Tema: Biblioteca<br>
Objetivo: Um aplicativo para ajudar na gestão de uma biblioteca<br>
Tecnologias: C# e Banco de Dados<br>
Descrição: Um app para desktop que auxilia o gerenciamento de uma biblioteca, tanto na parte administrativa, gerenciando o cadastro de livros e controle de estoque, quanto na parte da freguesia, onde será possível visualizar a disponibilidade dos livros, o agendamento, e a devolução.<br><br>

<h2>Requisitos Funcionais:</h2><br>
-senhas<br>
-classificação<br>
-cadastro<br>
-inserção livros<br>
-remover livros<br>
-emprestar livros<br>
-recuperação de senha<br>
-catalogo<br>
-ver se está disponível<br>
-agendar livros<br><br>

<h2>Requisitos não Funcionais:</h2><br>
-layout limpo e com pouca poluição visual<br>
-personalização<br>
-comentário<br>
-algoritimo de recomendação<br>
-avaliação do livro<br><br>

<h2>Quem vai usar:</h2><br>
administradores de biblioteca e clientes<br><br>


<h2>Caso de uso:</h2><br><br>

Entrar no sistema<br>
escolher se é administrador ou cliente<br><br>

```mermaid
graph LR
    classDef actor fill:#e1f5fe,stroke:#0288d1,stroke-width:2px;
    classDef common fill:#f3e5f5,stroke:#7b1fa2,stroke-width:1px;
    classDef admin fill:#fff3e0,stroke:#f57c00,stroke-width:1px;

    U[👤 Usuário Comum]:::actor
    A[👑 Administrador]:::actor

    subgraph Consultas e Empréstimos
        UC1(Filtrar por Gênero):::common
        UC2(Verificar Disponibilidade):::common
        UC3(Realizar Empréstimo):::common
    end

    subgraph Gestão e Estoque
        UC4(Acessar Aba de Cadastro):::admin
        UC5(Visualizar Estoque):::admin
        UC6(Cadastrar Novo Livro):::admin
        UC7(Remover Livro):::admin
    end

    U --> UC1
    U --> UC2
    U --> UC3

    A --> UC1
    A --> UC2
    A --> UC3
    A --> UC4
    A --> UC5
    A --> UC6
    A --> UC7



<h2>Telas</h2><br>

-Login<br>
-catalogo<br>
-cadastro/remoção de livros<br>
-visualização de estoque<br>
-agendar<br>
-recuperar senha<br>
