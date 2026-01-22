<p align="center">
  <img 
    src="https://github.com/user-attachments/assets/e4df3eda-e3de-4f05-8642-9a14de4f0e37"
    width="200"
    alt="image"
  />
</p>

##  Sobre

Este repositório apresenta o projeto **Cinema App**, desenvolvido como parte do desafio final do programa de estágio **AWS & AI for Software Quality Engineering**, com foco em **Quality Assurance (QA)**, testes manuais e automatizados.


 **Documentação completa, escopo detalhado e histórico do projeto** estão disponíveis no repositório original no Bitbucket:  
🔗 https://bitbucket.org/cinematests/cinema_app_final_challenge/src/main/



<p align="center">
  <img 
    src="https://github.com/user-attachments/assets/4790570c-71f0-4ae7-83cc-f4a622a3a54c"
    width="621"
    alt="image"
  />
</p>




## Introdução


Este repositório apresenta o projeto Cinema App, desenvolvido como parte do desafio final do programa de estágio AWS & AI for Software Quality Engineering. A aplicação base foi originalmente criada por [juniorschmitz](https://github.com/juniorschmitz) e serviu como plataforma para aplicação prática de testes de software.

O escopo do desafio consistiu em assumir o papel de Quality Assurance (QA) com foco na elaboração e execução de testes manuais e automatizados, cobrindo funcionalidades críticas da aplicação. As atividades envolveram:

- Planejamento de testes baseado em requisitos e heurísticas

- Criação de mapas mentais

- Documentação (Planos de Teste, Arquivo de Prompt, Relatórios)

- Execução de Testes (Manuais + Automatizados)

- Implementação de cenários de teste 

- Validação de APIs e fluxos do front-end

- Análise de falhas e reporte estruturado de bugs

- Adição de inovação no projeto


## Tecnologias 


- Robot Framework 
- Postman + QAlity 
- XMind
- Confluence 
- Jira 
- Git
- VSCode
- AI (OpenAI)
- MongoDB
- Trello
- Bitbucket



## Estrutura base 


A automação de testes foi estruturada em duas fases distintas, seguindo o princípio de separação de camadas: inicialmente voltada para a API (back-end) e, em seguida, para a interface do usuário (front-end). A organização do repositório reflete essa divisão, facilitando a manutenção, escalabilidade e compreensão do projeto.

```bash
cinema_app_final_challenge/

 backend-automation/
├── 📁 tests/                  # Casos de teste para APIs (Robot Framework, HTTP requests, validações)
├── 📁 keywords/               # Palavras-chave personalizadas para reuso em múltiplos testes
├── 📁 resources/              # Bibliotecas compartilhadas, setups, configurações
└── 📁 variables/              # Arquivos contendo variáveis comuns aos testes de backend

 frontend-automation/
├── 📁 tests/                  # Casos de teste para interface (UI), via browser automation (ex: Selenium, Playwright)
├── 📁 resources/
│   ├── 📁 page_objects/       # Padrão Page Object Model, com os mapeamentos das páginas da aplicação
│   └── common_keywords.robot  # Palavras-chave comuns utilizadas nos testes de frontend
└── 📁 variables/              # Variáveis específicas da automação de frontend

 results/                    # Pasta gerada com os relatórios de execução (.xml, .html, .log)

 README.md                   # Documentação do projeto, instruções de setup e execução
 
```


##  Recursos do Sistema


- Python 3.8 ou superior
- Node.js (necessário para o Browser Library)
- Navegador compatível com a [Browser Library](https://robotframework-browser.org/) (Chromium, Firefox, WebKit)


##  Pré-requisitos e Instalação


Siga os passos abaixo para configurar o ambiente local de testes:

1. **Clone o repositório**
   ```bash
   git clone <git clone git@bitbucket.org:cinematests/cinema_app_final_challenge.git>
   cd cinema_app_final_challenge
   ```

 3. **Instalar dependências**

 
**Com `requirements.txt`:**

```bash
pip install -r requirements.txt
```

Ou manualmente:


```bash
pip install robotframework
pip install robotframework-requests
```

4. **Executar os testes**

Execução padrão:


```bash
robot tests/
```

Com saída customizada (relatórios em results/):


```bash
robot -d results tests/
```


## Innovation Layer: Rastreabilidade Automatizada em CI/CD


Como diferencial técnico deste projeto, foi implementada uma **camada de inovação** voltada à rastreabilidade de QA integrada ao CI/CD. A automação conecta o **Bitbucket Pipelines** ao **Trello**, garantindo **visibilidade contínua do progresso de qualidade** sem esforço manual.

 **Cards Trello atualizados automaticamente** com base em ações no Git:
- **Commit em branch X** → card vai para `EXECUÇÃO`
- **Pull Request criado** → card move para `EM REVISÃO`
- **Merge na `main`** → card finalizado em `CONCLUÍDO`

 **Scripts e lógica inteligente**:
- Geração automática de cards se ausentes
- Checklists e descrições técnicas organizadas
- Mapeamento entre branches e tarefas via convenções como `plus/CINEMA-005-innovation-part`

 Essa abordagem **reduz erros humanos**, **aumenta a produtividade** e **fortalece a integração QA + Dev**, trazendo rastreabilidade real-time ao ciclo de vida dos testes.

 🔗 **Veja a implementação técnica completa no Bitbucket:**  
[Innovation Part - Branch `plus/CINEMA-005-innovation-part`](https://bitbucket.org/cinematests/cinema_app_final_challenge/src/54f85e3f634c0606a6781cf6fc92f2bf26feef3b/?at=plus%2FCINEMA-005-innovation-part)



---
###  Sobre a Autora


**Karen Késsia** é estagiária em **Quality Engineering**, apaixonada por **testes de software** e **análise de dados**. Com uma mente curiosa e comprometida com qualidade, ela busca tornar os produtos mais confiáveis, funcionais e acessíveis para os usuários.

<p align="center">
  <img 
    src="https://github.com/user-attachments/assets/6e506927-8c94-4964-b74d-4f3775c3e4a4"
    width="400"
  />
</p>

