# BIBLIOTEC

**Integrantes:** Bianca e Leonardo Agripino  
**Tema:** Gestão de Biblioteca  
**Tecnologias:** C# e Banco de Dados  

---

## Objetivo
Desenvolver um aplicativo desktop intuitivo para auxiliar na gestão de bibliotecas. O sistema atende tanto a administração — gerenciando o cadastro de livros e controle de estoque — quanto os clientes, permitindo consultar o catálogo, verificar disponibilidade e realizar agendamentos.

---

## Requisitos do Sistema

### Requisitos Funcionais (RF)
* **Autenticação:** Login seguro e recuperação de senha.
* **Gestão de Acervo:** Cadastro, edição, inserção e remoção de livros.
* **Consulta e Catálogo:** Visualização organizada com filtros por gênero e status de disponibilidade.
* **Operações de Usuário:** Empréstimo e agendamento de livros.

### Requisitos Não Funcionais (RNF)
* **Design:** Layout limpo e com poluição visual reduzida.
* **Experiência do Usuário:** Algoritmo de recomendação, sistema de avaliação de livros e campos de comentários.
* **Personalização:** Opções para ajustar a interface conforme a necessidade.

---

## Perfis de Usuário
* **Administrador:** Acesso total à gestão de estoque e cadastro de itens.
* **Cliente:** Acesso à consulta de acervo, agendamento e disponibilidade.

---

## Diagrama de Caso de Uso

```mermaid
graph TD
    classDef actor fill:#e1f5fe,stroke:#0288d1,stroke-width:2px;
    classDef usecase fill:#f3e5f5,stroke:#7b1fa2,stroke-width:1px;

    Admin[Administrador]:::actor
    User[Cliente / Usuário]:::actor

    subgraph Módulo de Acesso
        UC_Login(Entrar no Sistema / Login):::usecase
        UC_Recuperar(Recuperar Senha):::usecase
    end

    subgraph Módulo de Consulta
        UC_Catalogo(Navegar pelo Catálogo / Gênero):::usecase
        UC_Disp(Verificar Disponibilidade):::usecase
        UC_Agendar(Agendar / Emprestar Livro):::usecase
    end

    subgraph Módulo Administrativo
        UC_Estoque(Visualizar Estoque):::usecase
        UC_Cadastro(Cadastro / Remoção de Livros):::usecase
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
<h2>Telas</h2><br>

-Login<br>
-catalogo<br>
-cadastro/remoção de livros<br>
-visualização de estoque<br>
-agendar<br>
-recuperar senha<br>
Aplique aqui
