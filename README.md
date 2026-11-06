# 📊 ReportRepositories - Releases

Plataforma centralizada para monitoramento de serviços fiscais (SEFAZ), replicação de dados, gestão de infraestrutura de lojas, relatórios operacionais e distribuição de softwares.

---

**Última Versão:** \1.0.50\  
**Data de Publicação:** 06/11/2026 13:21  

[⬇️ Baixar Pacote Completo (v1.0.50)](https://github.com/gabriel-l96/ReportRepositories-Releases/releases/download/v1.0.50/ReportRepositories_v1.0.50.zip) · [📋 Histórico de Versões](https://github.com/gabriel-l96/ReportRepositories-Releases/releases)

---

## 🚀 Principais Funcionalidades

### 🏛️ Monitoramento de Disponibilidade SEFAZ
- **Documentos Fiscais Suportados:** NF-e (v4.00), NFC-e (v4.00) e CT-e (v4.00).
- **Cobertura Nacional Completa:** Autorizadores próprios (SP, MG, RS, MT, MS, PR, GO, etc.) e ambientes centralizados (SVRS, SVAN, SVSP, SVC-AN e SVC-RS).
- **Worker em Segundo Plano:** Varredura periódica e automática com medição de latência em milissegundos e retenção de histórico.
- **Dashboard em Tempo Real:** Painel visual com status por autorizador, filtros por UF/documento, histórico e gráficos de latência responsivos (temas Light e Dark).

### 🔄 Replicação, Infraestrutura e Monitoramento
- **Checagem de Replicação:** Monitoramento contínuo de sincronismo entre lojas, matriz e bancos de dados.
- **Checagem de Serviços:** Inspeção em tempo real de integradores, microserviços e serviços do Windows.
- **Contingência & Fecha Mês:** Acompanhamento de notas emitidas em contingência e rotinas de fechamento mensal.
- **Telemetria de Lojas:** Métricas de tráfego, status de conexão e latência das redes de lojas.
- **Dashboard de Auditoria:** Rastreamento de acessos e ações críticas no ecossistema.

### 🏢 Gestão de Redes, Acessos e Tags
- **Cadastro de Redes & Lojas:** Segmentação organizada por bandeira e unidade.
- **Cadastro de Conexões:** Gerenciamento seguro de rotas e credenciais de acesso aos servidores remotos.
- **Classificação por Tags:** Marcação de lojas e servidores para buscas, filtros e ações em massa.

### 📊 Relatórios & Scripts SQL
- **Repositório Central de Relatórios:** Criação, versionamento e execução centralizada de relatórios.
- **Distribuição de Scripts SQL:** Automação para envio e execução controlada de queries em bases distribuídas.

### 📦 Gestão e Distribuição de Versões
- **Publicação Centralizada:** Distribuição de instaladores, patches e atualizações de módulos de software.
- **Controle de Retenção & Módulos:** Regras de limpeza de versões antigas e acompanhamento de adesão de cada loja.

### 🏷️ Precificação & Regulação (CMED)
- **Tabela CMED:** Consulta, importação e conformidade de preços de medicamentos regulados pela ANVISA.

### 🛡️ Gestão de Acessos & Segurança
- **Autenticação Unificada:** Sessões seguras entre API e Web via JWT e Cookies.
- **RBAC (Controle por Papéis):** Permissões granulares de acesso por usuário e módulo.

### 🤖 Alertas & Mensageria
- **Notificações via WhatsApp:** Envio automatizado de avisos operacionais e alertas de incidentes.

---

## 💻 Arquitetura e Serviços
- **Web (Frontend):** ASP.NET Core Razor Pages (Porta padrão: \8000\)
- **API (Backend):** ASP.NET Core Minimal APIs / EF Core (Porta padrão: \5075\)
- **Deploy Nativo:** Execução como Windows Services (\ReportRepositories\ e \ReportRepositoriesApi\).

---

## 🛠️ Instalação Rápida
1. Baixe o pacote \ReportRepositories_v1.0.50.zip\ e extraia na máquina de destino.
2. Execute \scripts\instalar.bat\ como **Administrador**.
3. Ajuste as conexões e chaves nos arquivos:
   - \C:\ReportRepositories\Api\appsettings.Production.json\
   - \C:\ReportRepositories\Web\appsettings.Production.json\
4. Reinicie os serviços no Windows:
   \\\cmd
   sc stop ReportRepositoriesApi && sc start ReportRepositoriesApi
   sc stop ReportRepositories && sc start ReportRepositories
   \\\

## 🔑 Credenciais Iniciais Padrão
- **Usuário:** \dmin\
- **Senha:** \123456\
*(Recomenda-se alterar a senha imediatamente após o primeiro login)*
