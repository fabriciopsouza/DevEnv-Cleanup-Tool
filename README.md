#EM DESENVOLVIMENTO

# Windows dev environment cleaner
## DevEnv Cleanup Tool

Ferramenta segura para limpeza completa de ambientes de desenvolvimento Python/VS Code no Windows.

## 📌 Guia Rápido de Uso

1. Salve o arquivo como `dev_cleanup.bat`
2. Execute como Administrador
3. Siga as opções do menu:
   - Faça backup (opção 2)
   - Execute a limpeza (opção 3)
4. Reinicie o computador após conclusão

## ⚠️ Atenção! O Que Será Afetado

### Será Removido
- Python (instalações de usuário)
- Anaconda/Miniconda
- VS Code
- Ambientes virtuais Python
- Configurações relacionadas

### Será Preservado
- Python do sistema
- Outros programas instalados
- Arquivos do Windows
- Configurações do sistema

## 📋 Requisitos

- Windows 10 ou 11
- Privilégios de Administrador
- Mínimo 1GB de espaço livre
- Todos os programas Python/VS Code fechados

## 💿 Instalação e Execução

### Onde Salvar
```
Locais Recomendados:
C:\Scripts\dev_cleanup.bat
ou
%USERPROFILE%\Scripts\dev_cleanup.bat

NÃO salvar em:
C:\Windows\
C:\Program Files\
C:\Program Files (x86)\
```

### Como Executar
1. **Método Recomendado**:
   - Clique direito no arquivo
   - "Executar como administrador"

2. **Via Command Prompt**:
   ```batch
   cd C:\Scripts
   runas /user:Administrator "dev_cleanup.bat"
   ```

3. **Via PowerShell**:
   ```powershell
   Start-Process "C:\Scripts\dev_cleanup.bat" -Verb RunAs
   ```

## 🛡️ Medidas de Segurança

- Verificação de privilégios administrativos
- Proteção contra execução simultânea
- Verificação de espaço em disco
- Backup automático antes de modificações
- Proteção de diretórios do sistema
- Sistema de retry para operações críticas

## 🔄 Como Usar

### Antes de Executar
1. Feche todos os programas:
   - VS Code
   - Python/IDEs Python
   - Anaconda Navigator
   - Jupyter Notebooks

2. Verifique processos:
   - Python (python.exe)
   - VS Code (code.exe)
   - Anaconda (conda.exe)

3. Faça backup de:
   - Projetos importantes
   - Configurações personalizadas
   - Requirements dos projetos

### Opções do Menu
```
====================================
LIMPEZA DE AMBIENTE DE DESENVOLVIMENTO
====================================
1. Analisar instalações existentes
2. Backup das configurações
3. Desinstalar tudo automaticamente
4. Limpar registros e pastas manualmente
5. Verificar instalações do sistema
6. Limpar variáveis PATH
7. Verificar processos em execução
8. Sair
```

## 📊 Logs e Backup

### Localização
```
Logs:
%USERPROFILE%\Desktop\dev_cleanup_[DATA]_[HORA].log

Backup:
%USERPROFILE%\Desktop\dev_backup_[DATA]_[HORA]\
```

### Conteúdo do Backup
- Configurações VS Code
- Lista de extensões
- Ambientes virtuais
- PATH original
- Chaves de registro

## ❌ Solução de Problemas

### Erros Comuns

1. **"Acesso Negado"**
   - Execute como Administrador
   - Verifique permissões
   - Mova para diretório não protegido

2. **"Processos em Uso"**
   - Feche todos os programas relacionados
   - Use Task Manager para verificar
   - Reinicie se necessário

3. **"Falha na Desinstalação"**
   - Verifique o log
   - Use opção de limpeza manual
   - Reinicie e tente novamente

## 🔍 Verificação Pós-Limpeza

1. **Verifique Remoções**:
   ```batch
   where python
   where code
   where conda
   ```

2. **Verifique PATH**:
   ```batch
   echo %PATH%
   ```

3. **Verifique Diretórios**:
   - AppData\Local\Programs\Python
   - Anaconda3
   - AppData\Local\Programs\Microsoft VS Code

## 📝 Notas Importantes

- Sempre execute como Administrador
- Faça backup antes de começar
- Não interrompa o processo
- Reinicie após conclusão
- Mantenha os logs para referência

## 📄 Licença

Distribuído sob a licença MIT. Veja `LICENSE` para mais informações.
