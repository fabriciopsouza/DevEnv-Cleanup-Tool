# Windows dev environment cleaner

🧹 Uma ferramenta poderosa para limpeza completa de ambientes de desenvolvimento Python/VS Code no Windows

## Sobre

DevEnv Cleanup Tool é um script batch avançado para Windows que automatiza a limpeza completa de ambientes de desenvolvimento Python, incluindo múltiplas instalações Python, Anaconda, e VS Code. Ideal para desenvolvedores que precisam "resetar" seus ambientes de desenvolvimento ou remover instalações conflitantes.

## ✨ Características

- 🔍 Análise detalhada de instalações existentes
- 💾 Backup automático de configurações e extensões
- 🗑️ Desinstalação automática com verificação
- 🧹 Limpeza profunda de registros e diretórios
- 📝 Log detalhado de todas as operações
- ⚡ Execução silenciosa disponível
- 🛡️ Verificações de segurança

## 📋 Pré-requisitos

- Windows 10/11
- Privilégios de Administrador
- Conhecimento básico sobre os componentes a serem removidos

## 🚀 Uso

1. Baixe o script `cleanup.bat`
2. Execute como Administrador
3. Siga o menu interativo

```batch
Opções disponíveis:
1. Analisar instalações existentes
2. Backup das configurações
3. Desinstalar tudo automaticamente
4. Limpar registros e pastas manualmente
5. Verificar instalações do sistema
6. Sair
```

## ⚙️ Componentes Gerenciados

- Python (todas as versões)
- Anaconda/Miniconda
- VS Code
- Ambientes virtuais
- Pacotes pip
- Extensões VS Code
- Registros do Windows
- Variáveis de ambiente

## 📊 Logs

O script gera logs detalhados em:
```
%USERPROFILE%\Desktop\dev_cleanup_[DATA]_[HORA].log
```

## 🔒 Segurança

- Verificação de privilégios administrativos
- Confirmação antes de operações destrutivas
- Backup automático de configurações
- Verificações de erro em cada operação

## 🤝 Contribuindo

Contribuições são bem-vindas! Por favor, leia nosso guia de contribuição antes de submeter um PR.

### Como contribuir:

1. Faça um Fork do projeto
2. Crie sua Feature Branch (`git checkout -b feature/AmazingFeature`)
3. Commit suas mudanças (`git commit -m 'Add some AmazingFeature'`)
4. Push para a Branch (`git push origin feature/AmazingFeature`)
5. Abra um Pull Request

## 📝 TODO

- [ ] Adicionar suporte para mais IDEs
- [ ] Interface gráfica opcional
- [ ] Restauração de backup
- [ ] Modo silencioso via parâmetros
- [ ] Suporte para Visual Studio
- [ ] Relatório em HTML

## 📄 Licença

Distribuído sob a licença MIT. Veja `LICENSE` para mais informações.

## 👥 Autores

* **Seu Nome** - *Trabalho inicial*

## 🙏 Agradecimentos

* Comunidade Python Brasil
* Stack Overflow
* Microsoft Docs
