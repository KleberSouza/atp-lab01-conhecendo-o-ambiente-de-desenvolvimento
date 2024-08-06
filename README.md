# Lab 01 - Conhecendo o ambiente de desenvolvimento

Em nossa disciplina iremos trabalhar com a linguagem de programação C# e o editor de código Visual Studio Code (<https://code.visualstudio.com/>).

Para criar uma aplicação console em C# usando o Visual Studio Code, você precisa seguir alguns passos. Vamos começar com a configuração do ambiente e depois criar o programa.

## 1. Instalar o .NET SDK

- Primeiro, certifique-se de que o .NET SDK está instalado em seu sistema. Você pode baixá-lo do site oficial do .NET(<https://dotnet.microsoft.com/pt-br/download>).

## 2. Instalar o Visual Studio Code

- Se você ainda não tem o Visual Studio Code instalado, baixe e instale a partir do site oficial (<https://code.visualstudio.com/>).

### 2.1 Instalar a Extensão C# no Visual Studio Code

- Abra o Visual Studio Code e instale a extensão C# fornecida pela Microsoft:

  - Abra o Visual Studio Code.
  - Vá para a aba de Extensões (Ctrl+Shift+X).
  - Pesquise por "C#".
  - Instale a extensão C# da Microsoft.

## 3. Criar uma Aplicação Console

- Abra o terminal no Visual Studio Code:

  - Vá para Terminal > New Terminal ou use o atalho Ctrl+Shift+ ou Ctrl+'.
  - Navegue até o diretório onde você deseja criar o projeto.

- Crie um novo projeto do tipo console:

    ```sh
    dotnet new console -n lab01-conhecendo-o-ambiente-de-desenvolvimento
    ```

- Este comando cria um novo diretório chamado lab01-conhecendo-o-ambiente-de-desenvolvimento com os arquivos necessários para uma aplicação console.

- Abra o diretório do projeto no Visual Studio Code:

    ```sh
    cd lab01-conhecendo-o-ambiente-de-desenvolvimento
    code .
    ```

- Estrutura do Projeto

  - Após abrir o projeto no Visual Studio Code, você verá a estrutura básica do projeto:

    ```sh
    - lab01-conhecendo-o-ambiente-de-desenvolvimento.csproj
    - Program.cs
    ```

- Código Inicial no Program.cs. O arquivo Program.cs conterá um código semelhante a este:

```csharp
using System;

class Program
{
    static void Main(string[] args)
    {
        Console.WriteLine("Hello, World!");
    }
}
```

- Executar o Programa
  - No terminal integrado do Visual Studio Code, execute:

    ```sh
    dotnet run
    ```

  - Isso compilará e executará a aplicação, exibindo "Hello, World!" no console.

- Modificar o Código
  - Abra o arquivo Program.cs.
  - Modifique a linha Console.WriteLine("Hello, World!"); para:

    ```csharp
    Console.WriteLine("Hello, [Seu Nome]!");
    ```

  - Salve o arquivo e execute o programa novamente:

    ```sh
    dotnet run
    ```

  - Agora, você verá "Hello, [Seu Nome]!" no console.

## 4. Instalar o Git

- Se você ainda não tem o Git instalado, baixe e instale a partir do site oficial. (<https://git-scm.com/>).

### 4.1 Configurar o Git

4.1.1 Abra o terminal no Visual Studio Code:

- Vá para Terminal > New Terminal ou use o atalho Ctrl+Shift+.

4.1.2 Configure seu nome de usuário e email do Git:

```sh
git config --global user.name "Seu Nome"
git config --global user.email "seu-email@example.com"
```

### 4.2 Submissão

- Após completar a atividade, faça o commit das suas mudanças e empurre para o repositório remoto:

```sh
git add .
git commit -m "Personalize mensagem de Hello World"
git push origin main
```

## 5. Material Complemetar

- Para auxiliar no inicio da sua jornada na programação com C#, faça os seguintes tutoriais:
  - Introdução ao GitHub (<https://learn.microsoft.com/pt-br/training/modules/introduction-to-github/>)
  - Escrever seu primeiro código C# (<https://learn.microsoft.com/pt-br/training/modules/csharp-write-first/>)
  - Armazenar e recuperar dados usando valores literais e variáveis em C# (<https://learn.microsoft.com/pt-br/training/modules/csharp-literals-variables/>)
  - Executar formatação de cadeia de caracteres básica em C# (<https://learn.microsoft.com/pt-br/training/modules/csharp-basic-formatting/>)
  - Executar operações básicas em números em C# (<https://learn.microsoft.com/pt-br/training/modules/csharp-basic-operations/>)
  - Projeto guiado – Calcular e imprimir notas dos alunos (<https://learn.microsoft.com/pt-br/training/paths/get-started-c-sharp-part-1/?ns-enrollment-type=Collection&ns-enrollment-id=yz26f8y64n7k07>)
