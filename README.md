# Todo API

Este é um simples projeto de API Todo (Lista de Tarefas) desenvolvido em C# utilizando o framework ASP.NET Core e o Entity Framework Core para persistência de dados em memória.

## Pré-requisitos

Certifique-se de ter o seguinte instalado em sua máquina:

- .NET Core SDK 3.1 ou superior

## Como Executar

1. Clone este repositório para o seu ambiente local:
   git clone https://github.com/ebrauta/TodoAPI.git

2. Navegue até o diretório do projeto:
  cd TodoAPI

3. Execute o projeto utilizando o comando:
   dotnet run


A API estará disponível em `https://localhost:5001` por padrão.

## Endpoints

### Obter todas as tarefas
GET /todoitems

### Obter uma tarefa específica
GET /todoitems/{id}

### Criar uma nova tarefa
POST /todoitems

Corpo da requisição:

```json
{
  "name": "Título da Tarefa",
  "isComplete": "Se a tarefa foi completada ou não" (true or false)
}
```

### Atualizar uma tarefa existente
PUT /todoitems/{id}

Corpo da requisição:

```json
{
  "name": "Título da Tarefa",
  "isComplete": "Se a tarefa foi completada ou não" (true or false)
}
```

### Excluir uma tarefa
DELETE /todoitems/{id}


## Contribuindo
Sinta-se à vontade para abrir uma issue ou enviar um pull request se quiser contribuir para este projeto!

## Licença
Este projeto é licenciado sob a MIT License.
