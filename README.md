
<h1> #BIBLIOTEC</h1>

Integrantes: Bianca e Leonardo Agripino<br>
Tema: Biblioteca<br>
<h3>Objetivo:</h3> Um aplicativo para ajudar na gestão de uma biblioteca<br><br>
<h3>Tecnologias:</h3> C# e Banco de Dados<br><br>
<h3>Descrição:</h3> Um app para desktop que auxilia o gerenciamento de uma biblioteca, tanto na parte administrativa, gerenciando o cadastro de livros e controle de estoque, quanto na parte da freguesia, onde será possível visualizar a disponibilidade dos livros, o agendamento, e a devolução.<br><br>



<h3>Requisitos Funcionais:</h3><br>
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

<h3>Requisitos não Funcionais:</h3><br>
-layout limpo e com pouca poluição visual<br>
-personalização<br>
layout visual e intuitivo<br>
-algoritimo de recomendação<br>
-filtros dinamicos<br><br>


## Perfis de Usuário
* **Administrador:** Acesso total à gestão de estoque e cadastro de itens.
* **Cliente:** Acesso à consulta de acervo, agendamento e disponibilidade.



<h3> Diagrama de Caso de Uso</h3>

```mermaid
graph TD
    Admin[Administrador]
    User[Cliente / Usuário]

    subgraph Módulo de Acesso
        UC_Login(Entrar no Sistema / Login)
        UC_Recuperar(Recuperar Senha)
    end

    subgraph Módulo de Consulta
        UC_Catalogo(Navegar pelo Catálogo / Gênero)
        UC_Disp(Verificar Disponibilidade)
        UC_Agendar(Agendar / Emprestar Livro)
    end

    subgraph Módulo Administrativo
        UC_Estoque(Visualizar Estoque)
        UC_Cadastro(Cadastro / Remoção de Livros)
    end

    Admin --> UC_Login
    User --> UC_Login
    UC_Login --> UC_Recuperar

    User --> UC_Catalogo
    User --> UC_Disp
    User --> UC_Agendar

    Admin --> UC_Catalogo
    Admin --> UC_Disp
    Admin --> UC_Estoque
    Admin --> UC_Cadastro

```
<h3>Telas</h3><br>

-Login<br>
-catalogo<br>
-cadastro/remoção de livros<br>
-visualização de estoque<br>
-agendar<br>
-recuperar senha<br>
Aplique aqui
