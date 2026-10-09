# BlazorViaCep

Aplicação em Blazor WebAssembly para consultar endereço por CEP utilizando a API pública do ViaCEP.

## Funcionalidades

- Digitar um CEP
- Remover caracteres não numéricos automaticamente
- Validar quantidade de dígitos
- Consultar endereço via API do ViaCEP
- Exibir os dados retornados: CEP, logradouro, complemento, bairro, cidade, estado e DDD
- Exibir mensagem de erro quando o CEP for inválido ou a requisição falhar

## Tecnologias

- .NET 10
- Blazor WebAssembly
- C#
- HTTP via `HttpClient`

## Pré-requisitos

- .NET SDK 10.0 ou superior
- Visual Studio 2022 / VS Code com suporte ao .NET

## Como executar

1. Abra o terminal na pasta do projeto
2. Restaure os pacotes:

```bash
dotnet restore
```

3. Execute a aplicação:

```bash
dotnet run
```

4. Acesse a URL exibida no terminal, normalmente algo como:

```text
http://localhost:5000
```

## Estrutura do projeto

```text
BlazorViaCep/
├── Layout/
├── Pages/
│   ├── Home.razor
│   └── Endereço.cs
├── App.razor
├── Program.cs
├── BlazorViaCep.csproj
├── _Imports.razor
└── README.md
```

## Observações

A API consultada é a do ViaCEP:

```text
https://viacep.com.br/ws/{CEP}/json/
```

Exemplo:

```text
https://viacep.com.br/ws/01001000/json/
```

## Licença

Este projeto foi desenvolvido para fins de estudo e prática com Blazor.
