# Documentação - Ferramenta de Criação de Agentes de IA Muvecom

## Visão Geral

Esta ferramenta permite a criação de agentes de IA especializados para atendimento, desenvolvida para uso interno da Muvecom. Através de uma interface intuitiva, é possível configurar, testar e baixar agentes personalizados que se integram com as APIs da plataforma. Ele também conta com um agente de BI integrado a um segundo webhook, no mesmo arquivo que é baixado o agente no final.

## Campos de Configuração

<img width="1160" height="651" alt="2025-09-11-230047_1160x651_scrot" src="https://github.com/user-attachments/assets/528cdc50-9d82-4de1-b256-f9cd184290f1" />

### 1. Briefing (Arquivo DOCX - Opcional)

**Descrição:**  
Este campo permite o upload de um documento DOCX contendo instruções detalhadas para o agente. O documento serve como base principal para o comportamento e conhecimento do agente.

**Funcionalidade:**  
- Aceita apenas arquivos no formato DOCX
- As instruções do documento são processadas e incorporadas ao agente
- Fornece contexto específico sobre o domínio de atuação do agente

**Recomendações:**  
- Estruture o documento com títulos e subtítulos para melhor organização
- Inclua exemplos de interações esperadas
- Defina claramente o tom de voz e personalidade desejados

### 2. Token de Acesso *

**Descrição:**  
Campo obrigatório para autenticação nas APIs da plataforma Muvecom.

**Funcionalidade:**  
- Permite que o agente acesse os recursos e serviços da plataforma
- Valida a permissão do usuário para criar agentes
- Garante a segurança das operações

**Obtendo o Token:**  
- Contate o administrador do sistema
- O token é gerado individualmente para cada usuário
- Deve ser mantido em sigilo para evitar uso não autorizado

### 3. Prompt Complementar (Opcional)

**Descrição:**  
Instruções adicionais que complementam ou refinam o briefing principal.

**Funcionalidade:**  
- Permite ajustes finos no comportamento do agente
- Adiciona comandos específicos não cobertos pelo documento principal
- Pode ser usado para testar variações sem modificar o arquivo DOCX

**Exemplos de uso:**  
- Especificar formato de respostas
- Definir restrições adicionais
- Adicionar saudações ou mensagens padrão

### 4. Senha para Download *

**Descrição:**  
Campo obrigatório para baixar o agente após sua criação.

**Funcionalidade:**  
- Medida de segurança para controlar o acesso aos agentes
- Previne download não autorizado de agentes
- Registra quem realizou o download do agente

**Obtendo a Senha:**  
- Disponível apenas com os administradores do sistema
- Deve ser solicitada para cada download
- Pode variar entre diferentes agentes ou departamentos

## Botões de Ação

<img width="543" height="65" alt="2025-09-11-230908_543x65_scrot" src="https://github.com/user-attachments/assets/3fc975c0-1904-4dfc-82a6-04db2f202dc3" />

### Gerar Prompt

Processa todas as informações fornecidas (briefing, token e prompt complementar) para criar o agente personalizado.

### Testar Agente
Permite testar o agente antes do download final, verificando seu comportamento com base nas configurações fornecidas.

### Baixar Agente
Disponibiliza o agente para download após a inserção da senha de autorização fornecida pelos administradores.

## Fluxo de Trabalho Recomendado

1. Preparar o documento DOCX com o briefing completo
2. Obter o token de acesso com os administradores
3. Fazer upload do documento e inserir o token
4. Adicionar instruções complementares se necessário
5. Clicar em "Gerar Prompt" para criar o agente
6. Testar o agente com o botão "Testar Agente"
7. Solicitar a senha de download aos administradores
8. Baixar o agente finalizado

## Observações Importantes

- Todos os campos marcados com (*) são obrigatórios
- O agente só estará completamente funcional após a implantação no ambiente destino
- Em caso de erros, verifique se o token e a senha estão corretos
- Contate a equipe de suporte para problemas com tokens ou senhas
