# 📘 Assignment: Construindo APIs REST com FastAPI

## 🎯 Objective

Nesta tarefa, você aprenderá a construir APIs REST usando o framework FastAPI em Python. Você criará endpoints para gerenciar uma lista de tarefas (To-Do List), incluindo operações de criação, leitura, atualização e exclusão (CRUD).

## 📝 Tasks

### 🛠️ Tarefa 1: Configurar o Projeto FastAPI

#### Description
Configure um projeto FastAPI básico e crie seu primeiro endpoint. Instale as dependências necessárias e execute o servidor de desenvolvimento para verificar que tudo está funcionando corretamente.

#### Requirements
Completed program should:

- Instalar o FastAPI e o Uvicorn (servidor ASGI) usando pip
- Criar uma aplicação FastAPI básica
- Implementar um endpoint GET na rota raiz ("/") que retorne uma mensagem de boas-vindas
- Executar o servidor e acessar a documentação interativa automática em `/docs`
- Verificar que o endpoint responde corretamente


### 🛠️ Tarefa 2: Criar API CRUD para To-Do List

#### Description
Implemente uma API completa para gerenciar tarefas (To-Do items) com operações CRUD (Create, Read, Update, Delete). Use modelos Pydantic para validação de dados e armazene as tarefas em memória usando uma lista Python.

#### Requirements
Completed program should:

- Definir um modelo Pydantic `TodoItem` com campos: id (int), título (str), descrição (str, opcional), e concluída (bool)
- Implementar endpoint POST `/todos` para criar uma nova tarefa
- Implementar endpoint GET `/todos` para listar todas as tarefas
- Implementar endpoint GET `/todos/{todo_id}` para obter uma tarefa específica por ID
- Implementar endpoint PUT `/todos/{todo_id}` para atualizar uma tarefa existente
- Implementar endpoint DELETE `/todos/{todo_id}` para deletar uma tarefa
- Retornar códigos de status HTTP apropriados (200, 201, 404, etc.)
- Tratar erros adequadamente (ex: quando uma tarefa não é encontrada)
- Testar todos os endpoints usando a documentação interativa do FastAPI


### 🛠️ Tarefa 3: Adicionar Filtros e Validações

#### Description
Melhore sua API adicionando recursos de filtragem e validações mais robustas. Implemente parâmetros de consulta para filtrar tarefas e adicione validações personalizadas.

#### Requirements
Completed program should:

- Adicionar parâmetro de consulta ao endpoint GET `/todos` para filtrar tarefas concluídas/não concluídas
- Adicionar validação para garantir que o título da tarefa tenha pelo menos 3 caracteres
- Adicionar parâmetro de consulta para limitar o número de tarefas retornadas (paginação básica)
- Implementar tratamento de exceções personalizado com mensagens de erro descritivas
- Adicionar documentação aos endpoints usando docstrings para melhorar a documentação automática
- Testar todos os filtros e validações através da interface `/docs`
