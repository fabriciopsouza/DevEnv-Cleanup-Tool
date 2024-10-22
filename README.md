# Windows dev environment cleaner
## DevEnv Cleanup Tool

🧹 Uma ferramenta segura e robusta para limpeza completa de ambientes de desenvolvimento Python/VS Code no Windows

## ⚠️ Medidas de Segurança

Esta ferramenta foi desenvolvida com múltiplas camadas de proteção para garantir que apenas os componentes alvo sejam afetados:

- ✅ Proteção contra remoção de diretórios do sistema
- ✅ Verificação de processos críticos em execução
- ✅ Backup automático antes de qualquer modificação
- ✅ Preservação de caminhos essenciais do PATH
- ✅ Log detalhado de todas as operações
- ✅ Verificação de espaço em disco
- ✅ Proteção contra execuções simultâneas
- ✅ Verificação de privilégios administrativos

### 🛡️ O que o script NÃO faz:

- ❌ Não modifica instalações do sistema Windows
- ❌ Não remove Python instalado em C:\Program Files
- ❌ Não altera registros críticos do sistema
- ❌ Não modifica PATH do sistema Windows
- ❌ Não afeta outros programas instalados

## 🎯 Componentes Gerenciados

O script remove APENAS:
- Python (instalações de usuário)
- Anaconda/Miniconda
- VS Code
- Ambientes virtuais Python
- Configurações relacionadas

## 📋 Pré-requisitos

- Windows 10/11
- Privilégios de Administrador
- Mínimo 1GB de espaço livre
- Nenhum processo Python/VS Code em execução

## 🚀 Uso Seguro

1. **Preparação**:
   - Feche todos os programas Python/VS Code
   - Salve seu trabalho em editores de texto
   - Feche IDEs em execução

2. **Execução**:
   ```bash
   # Execute como Administrador
   cleanup.bat
   ```

3. **Opções Disponíveis**:
   1. Analisar instalações existentes
   2. Backup das configurações
   3. Desinstalar tudo automaticamente
   4. Limpar registros e pastas manualmente
   5. Verificar instalações do sistema
   6. Limpar variáveis PATH
   7. Sair

## 📊 Sistema de Logs

O script mantém logs detalhados de todas as operações:
```
%USERPROFILE%\Desktop\dev_cleanup_[DATA]_[HORA].log
```

### 📝 Informações Registradas:
- Timestamp de cada operação
- Componentes encontrados
- Tentativas de desinstalação
- Erros e avisos
- Modificações no PATH
- Backups realizados

## 💾 Sistema de Backup

Antes de qualquer modificação, o script cria backups em:
```
%USERPROFILE%\Desktop\dev_backup_[DATA]_[HORA]\
```

### 🗃️ Itens Incluídos no Backup:
- Configurações VS Code
- Lista de extensões
- Ambientes virtuais
- Pacotes pip instalados
- Ambientes Conda
- PATH original
- Chaves de registro relevantes

## ⚡ Recursos de Segurança

### Verificação de Processos
- Impede remoção se processos críticos estiverem rodando
- Lista processos que precisam ser fechados
- Permite ao usuário fechar processos manualmente

### Proteção de Diretórios
- Lista de diretórios protegidos que não podem ser modificados
- Verificação antes de cada operação de remoção
- Preservação de caminhos do sistema

### Gerenciamento do PATH
- Preserva caminhos essenciais do sistema
- Backup do PATH original
- Validação antes de aplicar modificações

## 🔄 Recuperação

Em caso de problemas:
1. Acesse a pasta de backup
2. Use os arquivos de backup para restaurar configurações
3. Reinstale componentes necessários
4. Restaure PATH se necessário

## ⚠️ Avisos Importantes

1. **Sempre faça backup** antes de executar
2. Execute **somente como Administrador**
3. Feche todos os programas relacionados
4. Tenha **espaço em disco** suficiente
5. Reinicie após a conclusão

## 🐛 Solução de Problemas

Se encontrar problemas:
1. Verifique os logs detalhados
2. Confirme que não há processos bloqueando
3. Verifique permissões de administrador
4. Garanta espaço em disco suficiente

## 📄 Licença

Distribuído sob a licença MIT. Veja `LICENSE` para mais informações.

## 🤝 Contribuindo

1. Faça um Fork
2. Crie sua Feature Branch
3. Teste exaustivamente
4. Envie um Pull Request

## 🔍 Validação de Segurança

O script foi testado para garantir:
- Não afeta componentes do sistema
- Preserva instalações críticas
- Mantém integridade do Windows
- Protege contra falhas de execução

Quer que eu transcreva também o código atualizado com todas estas proteções?
