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

graph TD
    subgraph Sistema de Biblioteca
        UC1[Visualizar Livros por Gênero]
        UC2[Verificar Disponibilidade]
        UC3[Emprestar Livro]
        UC4[Acessar Aba de Cadastro]
        UC5[Visualizar Estoque]
        UC6[Cadastrar Livro]
        UC7[Remover Livro]
    end

    User((Usuário))
    Admin((Administrador))

    User --> UC1
    User --> UC2
    User --> UC3

    Admin --> UC1
    Admin --> UC2
    Admin --> UC3
    Admin --> UC4
    Admin --> UC5
    Admin --> UC6
    Admin --> UC7


<h2>Telas</h2><br>

-Login<br>
-catalogo<br>
-cadastro/remoção de livros<br>
-visualização de estoque<br>
-agendar<br>
-recuperar senha<br>
