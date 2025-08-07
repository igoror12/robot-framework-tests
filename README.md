# 🤖 Testes de Automação com Robot Framework

Este repositório contém um projeto de automação de testes desenvolvido com **Robot Framework** e **SeleniumLibrary**, focado em testar as funcionalidades de cadastro e preenchimento de formulários do site **Organo**.

## 🌟 Visão Geral do Projeto

O objetivo deste projeto é demonstrar a capacidade de automatizar testes de interface de usuário (UI) em aplicações web. Ele simula interações de usuário para validar o fluxo de preenchimento de formulários e a criação de cards no site Organo, cobrindo cenários de sucesso e falha (preenchimento incorreto).

## 🚀 Tecnologias Utilizadas

*   **Robot Framework:** Um framework de automação genérico para testes de aceitação e automação de processos robóticos (RPA).
*   **SeleniumLibrary:** Uma biblioteca do Robot Framework que utiliza o Selenium WebDriver para interagir com navegadores web.
*   **Python 3.8+:** Linguagem de programação base para o Robot Framework.
*   **FakerLibrary:** Utilizada para gerar dados de teste fictícios (nomes, cargos, imagens).

## 🧪 Estrutura do Projeto

O projeto está organizado da seguinte forma para facilitar a manutenção e escalabilidade:

```
. 
├── tests/ 
│   ├── preenchimento_correto.robot 
│   └── preenchimento_incorreto.robot 
├── resources/ 
│   ├── pages/ 
│   │   └── cadastro.robot 
│   ├── shared/ 
│   │   └── setup_teardown.robot 
│   └── main.robot 
├── .gitignore 
├── README.md 
└── (arquivos de log e relatórios gerados)
```

*   `tests/`: Contém os arquivos de casos de teste (`.robot`).
    *   `preenchimento_correto.robot`: Casos de teste para cenários de preenchimento de formulário bem-sucedidos.
    *   `preenchimento_incorreto.robot`: Casos de teste para cenários de preenchimento de formulário com dados inválidos ou campos obrigatórios não preenchidos.
*   `resources/`: Contém arquivos de recursos reutilizáveis (palavras-chave, variáveis, etc.).
    *   `pages/`: Módulos que representam as páginas da aplicação, seguindo o padrão Page Object Model (POM).
        *   `cadastro.robot`: Contém as palavras-chave e seletores relacionados à página de cadastro.
    *   `shared/`: Recursos compartilhados entre diferentes testes.
        *   `setup_teardown.robot`: Define as configurações de inicialização e finalização dos testes (abrir/fechar navegador).
    *   `main.robot`: Arquivo principal de recursos que importa as bibliotecas e outros recursos.
*   `.gitignore`: Lista de arquivos e pastas a serem ignorados pelo Git (ex: logs, relatórios, caches).
*   `README.md`: Este arquivo, contendo a documentação do projeto.

## ⚙️ Pré-requisitos

Certifique-se de ter os seguintes softwares instalados em sua máquina:

*   [Python 3.8+](https://www.python.org/downloads/)
*   [pip](https://pip.pypa.io/en/stable/installation/)
*   [Robot Framework](https://robotframework.org/)
*   [SeleniumLibrary](https://robotframework.org/SeleniumLibrary/)
*   [FakerLibrary](https://robotframework.org/FakerLibrary/)
*   Um navegador web (ex: Google Chrome, Mozilla Firefox) e seu respectivo WebDriver (ex: [ChromeDriver](https://chromedriver.chromium.org/downloads)).

## 🚀 Como Executar os Testes

Siga os passos abaixo para configurar e executar os testes em sua máquina local:

### 1. Clone o repositório

Abra seu terminal ou prompt de comando e execute:

```bash
git clone https://github.com/igoror12/robot-framework-tests.git
cd robot-framework-tests
```

### 2. Instale as dependências

Navegue até o diretório do projeto e instale as bibliotecas Python necessárias:

```bash
pip install robotframework robotframework-seleniumlibrary robotframework-faker
```

### 3. Baixe o WebDriver do navegador

Certifique-se de ter o WebDriver compatível com a versão do seu navegador e adicione-o ao PATH do sistema ou coloque-o no diretório raiz do projeto.

### 4. Execute os testes

Para executar todos os testes, utilize o comando:

```bash
robot tests/
```

Para executar um arquivo de teste específico:

```bash
robot tests/preenchimento_correto.robot
```

Após a execução, os relatórios (`log.html`, `report.html`) serão gerados no diretório raiz do projeto.

## 🤝 Contribuição

Contribuições são bem-vindas! Se você tiver sugestões de melhoria, novas funcionalidades ou encontrar bugs, sinta-se à vontade para abrir uma issue ou enviar um pull request.

## 📧 Contato

Para dúvidas ou informações adicionais, entre em contato com [igoror12](https://github.com/igoror12).


