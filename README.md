# Projeto de Automação - DemoQA

Este projeto tem como objetivo realizar testes automatizados na plataforma DemoQA utilizando Python, Playwright, Pytest e BDD (Gherkin). O foco é automatizar cenários funcionais da aplicação para validar comportamentos da interface, fluxos de usuário e interações com elementos da página. A aplicação utilizada para testes é: https://demoqa.com/

```bash
Automa-o-Playwright/
│
├── features/
│
├── tests/
│
├── steps/
│
├── pages/
│
├── utils/
│  ├── helpers. py
│  └── data_generator. py
│
├── config/
│  └── settings. py
│
├── conftest. py
├── pytest.ini
├── requirements.txt
├── .gitignore
└── README. md
```

## Documentação de Requisitos

Foi criado o arquivo
requisitos.md
com o objetivo de documentar os requisitos funcionais e não funcionais da aba Elements da aplicação. Este documento serve como base para a definição dos cenários BDD e auxilia na rastreabilidade entre as regras de negócio e os testes automatizados implementados no projeto.

 projeto segue o padrão Page Object Model, com separação de cenários BDD, implementação de steps, utilitários auxiliares, evidências de falha e relatórios de execução.

Para configurar o ambiente, crie um ambiente virtual com o comando:
bash
python -m venv venv
Ative o ambiente virtual:
bash
venv\Scripts\activate
As dependências estão definidas no arquivo requirements.txt:

**pytest** → Framework para execução de testes.  
**pytest-playwright** → Integração do Playwright com o Pytest.  
**allure-pytest** → Integração do Allure para geração de relatórios.  
**pytest-bdd** → Adiciona suporte à linguagem BDD aos testes.  
**pytest-rerunfailures** → Permite reexecutar testes que falharam.  
**pytest-xdist** → Permite a execução de testes em paralelo.  
**faker** → Biblioteca para geração de dados falsos, útil para testes.  
**locust** → Ferramenta de teste de carga para simular múltiplos usuários.  
**playwright** → Automação de navegadores para testes end-to-end.

Instale as dependências:
bash
pip install -r requirements.txt
Instale os navegadores do Playwright:
bash
playwright install
Para executar os testes:
bash
pytest
Para executar exibindo o navegador e logs detalhados:
bash
pytest --headed
Para abrir o relatório interativo:
bash
allure serve allure-results

#

# Registro de Bugs

Os bugs identificados durante a execução dos testes ou durante a análise da aplicação são registrados no próprio repositório do GitHub.

Eles podem ser visualizados e acompanhados através da aba "Issues", onde são documentados com descrição do problema, passos para reprodução, evidências e informações do ambiente. 

https://github.com/DanilogLuz/Automa-o/issues

#


# Integração Contínua (CI)

O projeto possui integração contínua utilizando GitHub "Actions".

O workflow está definido no arquivo: .github/workflows/CI.yml


#



Desenvolvido por Danilo Luz.

Charles Leclerc

testesabonete
