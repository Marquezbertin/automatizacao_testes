# Automação de Testes com Selenium IDE

![GitHub repo size](https://img.shields.io/github/repo-size/Marquezbertin/automatizacao_testes)
![GitHub language](https://img.shields.io/github/languages/count/Marquezbertin/automatizacao_testes)
![GitHub last commit](https://img.shields.io/github/last-commit/Marquezbertin/automatizacao_testes)
![GitHub issues](https://img.shields.io/github/issues/Marquezbertin/automatizacao_testes)
![GitHub forks](https://img.shields.io/github/forks/Marquezbertin/automatizacao_testes)

## Sobre

Este repositório contém exemplos de automação de testes de interface usando **Selenium IDE** (arquivos `.side`). Os scripts foram desenvolvidos para testar funcionalidades do site **Demo Fire** (banco simulado) e servem como base para aprender e praticar testes de automação.

## Estrutura

```
automatizacao_testes/
├── README.md            # Documentação do projeto
├── config.json          # Configurações gerais
├── ferramentas.md       # Ferramentas auxiliares
├── banco_altoromutual/
│   ├── README.MD        # Documentação do módulo bancário
│   ├── scripts/         # Scripts de teste (.side - Selenium IDE)
│   │   ├── IBM BANKING_LOGIN.side
│   │   ├── aba_localizacao.side
│   │   ├── detalhes_conta.side
│   │   ├── email_informações_produtos.side
│   │   ├── seguro_vida_error.side
│   │   └── transferência_extrato.side
│   └── screenshots/     # prints de tela dos testes executados
└── .github/
    └── workflows/
        └── validate.yml # Validação de arquivos .side
```

## Scripts de Teste

Cada script `.side` é um arquivo JSON que define os passos de um teste no Selenium IDE. Os scripts disponíveis:

| Script | Descrição |
|--------|-----------|
| `IBM BANKING_LOGIN.side` | Teste de login no sistema bancário |
| `aba_localizacao.side` | Teste que alterna entre abas do navegador |
| `detalhes_conta.side` | Teste de visualização de detalhes da conta |
| `email_informações_produtos.side` | Teste de inscrição em e-mails de produtos |
| `seguro_vida_error.side` | Teste de validação de erro ao incluir seguro de vida |
| `transferência_extrato.side` | Teste de transferência e extrato bancário |

## Como executar

### 1. Instalar o Selenium IDE

- **Firefox:** Acesse a [Firefox Add-ons](https://addons.mozilla.org/pt-BR/firefox/add/selenium-ide/) e clique em "Adicionar ao Firefox".
- **Chrome:** Acesse a [Chrome Web Store](https://chrome.google.com/webstore/detail/selenium-ide) e clique em "Adicionar ao Chrome".

### 2. Importar e executar

1. Abra o Selenium IDE.
2. Clique em **File > Open project...** e selecione a pasta `banco_altoromutual/scripts`.
3. Selecione o teste desejado na lista.
4. Clique em **Play current test** para executar.

### 3. (Opcional) Executar via linha de comando

```bash
# Instalar o runner globalmente (npm)
npm install -g selenium-ide-runner

# Executar um teste específico
selenium-ide-runner -c "chrome" banco_altoromutual/scripts/IBM\ BANKING_LOGIN.side
```

## Contribuindo

1. **Fork** o repositório.
2. Crie uma branch (`git checkout -b feature/novo-teste`).
3. Adicione um novo arquivo `.side` na pasta `banco_altoromutual/scripts/`.
4. Commit suas alterações (`git commit -m 'add: novo teste de automação'`).
5. Push para a branch (`git push origin feature/novo-teste`).
6. Abra um **Pull Request**.

## Licença

Este projeto está licenciado sob a licença MIT. Veja o arquivo [LICENSE](LICENSE) para mais detalhes.

---

Feito com 🤍 por Bruno Bertin Marquez – Analista de QA.

---

## Citação e DOI

[![DOI](https://zenodo.org/badge/DOI/10.5281/zenodo.24163215.svg)](https://doi.org/10.5281/zenodo.24163215)
[![ORCID](https://img.shields.io/badge/ORCID-0009--0005--3546--8302-A6CE39?logo=orcid&logoColor=white)](https://orcid.org/0009-0005-3546-8302)

- **Zenodo (DOI):** https://doi.org/10.5281/zenodo.24163215
- **ORCID:** https://orcid.org/0009-0005-3546-8302
