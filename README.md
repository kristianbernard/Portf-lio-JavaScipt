
# Documentação do Formulário de E-mail

## Introdução

Este projeto consiste em um formulário dinâmico para a coleta de endereços de e-mail, desenvolvido com HTML, Bootstrap e JavaScript para validação no lado do cliente. O objetivo da validação é garantir que os e-mails inseridos sigam um formato adequado antes do processamento.

## Tecnologias Utilizadas
- HTML5: Estruturação da página.
- Bootstrap 5.3: Estilização e componentes interativos.
- JavaScript: Validação do campo de e-mail e exibição de mensagens em um modal.

## Estrutura do Projeto

#### Formulário de E-mail

O formulário contém:
- Um campo de entrada para o e-mail.
- Um botão para envio dos dados.

#### Validação

A validação é realizada em JavaScript utilizando a seguinte expressão regular:

```http
  /^[a-zA-Z0-9._-]+@[a-zA-Z0-9.-]+\.[a-zA-Z]{2,}$/
```

Essa expressão verifica se o e-mail está no formato correto, como "exemplo@dominio.com".

## Exibição de Mensagens

As mensagens de erro ou sucesso são apresentadas em um modal Bootstrap. As verificações incluem:
- **Campo vazio**: "O campo de e-mail não pode estar vazio."
- **Formato incorreto**: "Por favor, insira um e-mail válido."
- **Formato válido**: "E-mail válido! Formulário enviado com sucesso."

## Funcionamento

    1. O usuário insere um e-mail no campo de entrada.
    2. Ao clicar no botão "Enviar", o JavaScript executa a validação:
         - Se o campo estiver vazio ou o formato for inválido, uma mensagem de erro será exibida no modal.
         - Caso seja um e-mail válido, uma mensagem de sucesso será apresentada.

## Dependências

O projeto faz uso do Bootstrap via CDN:

```http
  <link href="https://cdn.jsdelivr.net/npm/bootstrap@5.3.0/dist/css/bootstrap.min.css" rel="stylesheet">
  <script src="https://cdn.jsdelivr.net/npm/bootstrap@5.3.0/dist/js/bootstrap.bundle.min.js"></script>
```

## Conclusão

Este projeto demonstra boas práticas na validação de formulários web, proporcionando uma experiência de usuário aprimorada e minimizando erros de entrada de dados.
