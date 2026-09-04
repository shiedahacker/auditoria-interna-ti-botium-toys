# 🔐 Auditoria Interna de TI — Botium Toys

> Projeto de portfólio em Cibersegurança baseado no curso **"Play It Safe: Manage Security Risks"**, parte do **Google Cybersecurity Certificate**.

![Cybersecurity](https://img.shields.io/badge/Cybersecurity-Project-red)
![NIST CSF](https://img.shields.io/badge/Framework-NIST%20CSF-blue)
![GDPR](https://img.shields.io/badge/Compliance-GDPR-green)
![PCI DSS](https://img.shields.io/badge/Compliance-PCI%20DSS-orange)

---

## 📌 Sobre o projeto

Este projeto consiste em uma **auditoria interna de TI** realizada em uma empresa fictícia chamada **Botium Toys**.

O objetivo da auditoria foi avaliar a postura de segurança da organização, identificar riscos e deficiências nos controles existentes e propor recomendações para reduzir os riscos identificados.

A análise foi desenvolvida com base nos conceitos estudados no curso **Play It Safe: Manage Security Risks**, do **Google Cybersecurity Certificate**, utilizando como referências os princípios de segurança da **OWASP** e o **NIST Cybersecurity Framework (NIST CSF)**.

---

## 🎯 Objetivos

A auditoria teve como principais objetivos:

- Avaliar os ativos atualmente gerenciados pelo departamento de TI;
- Identificar riscos de segurança;
- Avaliar controles existentes;
- Identificar gaps de segurança e conformidade;
- Priorizar os controles que necessitam de implementação;
- Mapear os principais achados ao NIST Cybersecurity Framework;
- Apresentar recomendações para melhoria da postura de segurança.

---

## 🏢 Cenário

A **Botium Toys** é uma pequena empresa dos Estados Unidos que desenvolve e comercializa brinquedos.

A empresa possui uma unidade física que funciona como:

- Escritório;
- Loja;
- Depósito.

Com o crescimento da operação online e a expansão para clientes internacionais, a área de TI passou a enfrentar novos desafios relacionados à:

- Segurança da informação;
- Proteção de dados;
- Controle de acessos;
- Continuidade operacional;
- Segurança dos pagamentos;
- Conformidade regulatória.

---

## 📦 Ativos analisados

Durante a auditoria foram considerados diferentes tipos de ativos e recursos de TI, incluindo:

- Equipamentos locais (*on-premises*);
- Desktops e notebooks;
- Smartphones;
- Estações de trabalho remotas;
- Equipamentos e periféricos;
- Câmeras de vigilância;
- Sistemas e aplicações;
- Bancos de dados;
- Sistemas de comércio eletrônico;
- Sistemas de gestão de estoque;
- Rede interna;
- Acesso à Internet;
- Armazenamento e retenção de dados;
- Sistemas legados.

---

# ⚠️ Avaliação de riscos

Os riscos foram classificados considerando **probabilidade, impacto e severidade**.

| Ativo / Área | Ameaça / Risco | Probabilidade | Impacto | Severidade |
|---|---|---:|---:|---:|
| Sistemas legados | Exploração de vulnerabilidades não corrigidas | Alta | Alto | 🔴 Crítico |
| Contas de usuário | Acesso indevido por ausência de privilégio mínimo | Alta | Médio | 🟠 Alto |
| Dados de cartão de pagamento | Vazamento de dados / não conformidade PCI DSS | Média | Alto | 🟠 Alto |
| Dados pessoais de clientes da UE | Multas por não conformidade com GDPR | Média | Alto | 🟠 Alto |
| Continuidade operacional | Indisponibilidade por ausência de DRP e backups | Média | Alto | 🟠 Alto |
| Endpoints | Infecção por malware sem AV/EDR ativo | Alta | Médio | 🟠 Alto |

---

# 🛡️ Controles avaliados

Durante a auditoria foram analisados diferentes controles de segurança e conformidade.

| Controle | Status | Prioridade |
|---|---|---:|
| Privilégio mínimo e segregação de funções | ❌ Não implementado | 🔴 Crítica |
| Plano de recuperação de desastres (DRP) | ❌ Não implementado | 🔴 Crítica |
| Políticas de senha e gestão de contas | ⚠️ Inconsistente | 🔴 Crítica |
| Sistema de detecção de intrusão (IDS) | ❌ Não implementado | 🔴 Crítica |
| Criptografia em transações online | ⚠️ A verificar | 🔴 Crítica |
| Backups | ❌ Não implementado | 🔴 Crítica |
| Antivírus / EDR | ❌ Não implementado | 🔴 Crítica |
| Gerenciamento de senhas | ❌ Não implementado | 🔴 Crítica |
| Conformidade com GDPR | ⚠️ Parcial | 🟠 Alta |
| Conformidade com PCI DSS | ⚠️ Parcial | 🟠 Alta |
| Diretrizes SOC 1 / SOC 2 | ⚠️ Parcial | 🟡 Média |
| Sinalização de segurança física | ❌ Não implementado | 🟢 Baixa |

---

# 🚨 Principais recomendações

Com base nos riscos identificados, foram propostas as seguintes medidas:

### 🔑 Controle de acesso

- Aplicação do princípio do menor privilégio;
- Revisão das permissões dos usuários;
- Implementação de RBAC;
- Segregação de funções;
- Implementação de MFA;
- Formalização de políticas de senha;
- Desativação de contas inativas;
- Implantação de gerenciador corporativo de senhas.

### 🛡️ Proteção de endpoints

- Implantação de solução de antivírus / EDR;
- Monitoramento contínuo dos endpoints;
- Atenção especial aos sistemas legados.

### 🔎 Detecção

- Implantação de IDS/IPS;
- Monitoramento contínuo;
- Integração de mecanismos de detecção à infraestrutura existente.

### 💾 Continuidade

- Criação de um Plano de Recuperação de Desastres (DRP);
- Implementação de backups automatizados;
- Realização de testes de restauração.

### 🔐 Proteção de dados

- Garantir TLS 1.2+ no tráfego do e-commerce;
- Revisar o tratamento de dados pessoais;
- Avaliar os controles relacionados aos dados de cartão.

### 📋 Governança e conformidade

- Mapear dados pessoais de clientes da União Europeia;
- Formalizar políticas de tratamento de dados;
- Validar o escopo de PCI DSS;
- Avaliar a segmentação da rede de pagamentos;
- Formalizar controles de acesso de terceiros e fornecedores.

---

# 🧠 Mapeamento ao NIST Cybersecurity Framework

Os principais achados da auditoria foram relacionados às cinco funções centrais do **NIST CSF**.

| NIST CSF | Aplicação no projeto |
|---|---|
| 🔎 **Identify** | Inventário de ativos e avaliação de riscos |
| 🛡️ **Protect** | Privilégio mínimo, MFA, gerenciamento de senhas, criptografia e controles de acesso |
| 🚨 **Detect** | IDS e antivírus / EDR |
| 🧯 **Respond** | Políticas, procedimentos e playbooks de resposta a incidentes |
| ♻️ **Recover** | DRP, backups e testes de restauração |

---

# 📋 Conformidade analisada

## GDPR

Foi considerada a necessidade de adequação relacionada ao tratamento de dados pessoais de clientes da União Europeia.

## PCI DSS

Foi analisada a necessidade de controles relacionados ao processamento e armazenamento de dados de cartões de pagamento.

## SOC 1 / SOC 2

Foram consideradas diretrizes relacionadas a controles de acesso, fornecedores e proteção das informações.

---

# 📊 Priorização

As descobertas críticas identificadas pela auditoria incluem:

1. Privilégio mínimo e segregação de funções;
2. Plano de recuperação de desastres;
3. Políticas de senha e gestão de contas;
4. Sistema de detecção de intrusão;
5. Criptografia das transações online;
6. Backups;
7. Antivírus / EDR;
8. Gerenciamento de senhas.

Esses pontos foram classificados como de **tratamento imediato** na auditoria.

---

# 🎓 Competências demonstradas

Este projeto permitiu aplicar conceitos relacionados a:

- 🔐 Gestão de riscos de segurança;
- 🛡️ Controles de segurança;
- 🔎 Avaliação de vulnerabilidades e gaps;
- 📋 Auditoria interna de TI;
- 🧠 NIST Cybersecurity Framework;
- 🔑 Controle de acesso e menor privilégio;
- 🚨 Detecção de ameaças;
- 💾 Continuidade de negócio;
- 📊 Priorização de riscos;
- 📑 Compliance e governança;
- GDPR;
- PCI DSS;
- SOC 1 / SOC 2.

---

# 📄 Documentação completa

A documentação completa da auditoria está disponível no arquivo abaixo:

👉 **[📄 Visualizar Auditoria Interna de TI — Botium Toys](./documentos/Auditoria_Botium_Toys.pdf)**

---

# 📚 Referências

- Google Cybersecurity Certificate — *Play It Safe: Manage Security Risks*
- NIST Cybersecurity Framework
- OWASP
- GDPR
- PCI DSS
- SOC 1 / SOC 2

---

## 👨‍💻 Autor

**Jose Italo**

🔐 Cybersecurity Student  
🛡️ SOC | Blue Team  
📊 Security & Risk Management

GitHub: [@shiedahacker](https://github.com/shiedahacker)
