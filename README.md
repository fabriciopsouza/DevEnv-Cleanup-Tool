# Windows dev environment cleaner
## DevEnv Cleanup Tool

Ferramenta segura e robusta para limpeza completa de ambientes de desenvolvimento Python/VS Code no Windows, com verificações aprimoradas e sistema de retry.

## ⚡ Guia Rápido

```plaintext
1. Execute como Administrador
2. Verifique compatibilidade com Windows 10/11
3. Faça backup (opção 2)
4. Execute limpeza (opção 3)
5. Reinicie o sistema
```

## 🛡️ Recursos de Segurança Aprimorados

### Verificações Automatizadas
- Detecção precisa da versão do Windows
- Sistema robusto de lock com informações detalhadas
- Verificação aprimorada de processos em execução
- Backup do registro antes de modificações
- Sistema de retry com descrições detalhadas

### Proteções do Sistema
- Verificação multinível de processos críticos
- Backup do PATH com timestamp
- Confirmação interativa para operações críticas
- Log detalhado de todas as operações
- Histórico de backups do PATH

## 📋 Pré-requisitos

- Windows 10 ou 11 (verificação automática)
- Privilégios de Administrador
- 1GB de espaço livre mínimo
- Processos Python/VS Code encerrados

## 🚀 Funcionalidades Aprimoradas

### Verificação de Processos
- Lista detalhada de processos em execução
- Opções flexíveis de tratamento:
  - [S] Aguardar fechamento
  - [C] Cancelar operação
  - [N] Prosseguir assim mesmo

### Sistema de Retry
- Tentativas configuráveis (padrão: 3)
- Delay entre tentativas ajustável
- Mensagens descritivas para cada operação
- Log detalhado de falhas

### Gestão do PATH
- Backup com timestamp
- Histórico de modificações
- Verificação de integridade
- Restauração facilitada

## 📊 Sistema de Logs Aprimorado

### Informações Registradas
- Timestamp preciso
- Usuário executor
- Versão do Windows
- Processos detectados
- Operações realizadas
- Tentativas de retry
- Modificações no PATH

### Localização
```
%USERPROFILE%\Desktop\dev_cleanup_[TIMESTAMP].log
```

## 🔄 Processo de Desinstalação

### Python
1. Backup do registro
2. Lista versões instaladas
3. Confirmação específica
4. Desinstalação com retry
5. Verificação pós-remoção

### VS Code
1. Verificação de processos
2. Backup de configurações
3. Desinstalação silenciosa
4. Retry em caso de falha
5. Limpeza de resíduos

### Anaconda
1. Detecção de ambientes
2. Backup de configurações
3. Desinstalação automática
4. Verificação de PATH
5. Limpeza de diretórios

## ⚙️ Menu Aprimorado

```plaintext
====================================
LIMPEZA DE AMBIENTE DE DESENVOLVIMENTO
====================================
Data/Hora: [atual]
Usuário: [logado]
Log: [caminho]

1. Analisar instalações existentes
2. Backup das configurações
3. Desinstalar tudo automaticamente
4. Limpar registros e pastas manualmente
5. Verificar instalações do sistema
6. Limpar variáveis PATH
7. Verificar processos em execução
8. Sair
```

## 🔍 Verificações de Segurança

### Antes da Execução
- Versão do Windows compatível
- Espaço em disco suficiente
- Privilégios adequados
- Lock file disponível

### Durante a Execução
- Monitoramento de processos
- Verificação de path protegidos
- Validação de operações críticas
- Sistema de retry em falhas

### Pós-Execução
- Verificação de remoção
- Validação do PATH
- Integridade do sistema
- Logs completos

## 🆘 Tratamento de Erros

### Retry Automatizado
- Tentativas configuráveis
- Delay entre tentativas
- Descrição detalhada
- Log de falhas

### Recuperação
- Backups com timestamp
- Histórico do PATH
- Registro de operações
- Scripts de restauração

## 📝 Logs e Relatórios

### Conteúdo
- Operações realizadas
- Erros encontrados
- Tentativas de retry
- Modificações no sistema
- Backups criados

### Formato
- Timestamp preciso
- Descrições detalhadas
- Status de operações
- Caminhos afetados

## 🔐 Recomendações de Uso

1. Sempre execute como Administrador
2. Verifique processos em execução
3. Faça backup antes de iniciar
4. Mantenha logs para referência
5. Reinicie após conclusão

## 🛠️ Configurações Avançadas

Ajuste no início do script:
```batch
set "MAX_RETRIES=3"
set "RETRY_DELAY=5"
set "MIN_DISK_SPACE=1073741824"
```

## 📄 Licença

MIT License - Veja LICENSE para detalhes

---

**Nota**: Esta versão inclui melhorias significativas no tratamento de erros, verificação de processos e sistema de backup. Sempre verifique o log para detalhes completos das operações realizadas.
