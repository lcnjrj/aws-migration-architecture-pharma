# 💊 AWS Cloud Migration: Pharma Distribution Hub

![AWS](https://img.shields.io/badge/AWS-Cloud-orange?style=for-the-badge&logo=amazon-aws&logoColor=white)
![Architecture](https://img.shields.io/badge/Architecture-High%20Availability-blue?style=for-the-badge)
![Status](https://img.shields.io/badge/Status-Proposed-green?style=for-the-badge)

## 📋 Resumo Executivo
Projeto de consultoria para transformação digital de um Hub de Distribuição Farmacêutica no Rio de Janeiro (280 funcionários). O objetivo foi desenhar uma arquitetura de nuvem AWS que viabilizasse a expansão nacional, reduzisse custos fixos (CAPEX) e mitigasse riscos de infraestrutura (falhas de energia).

---

## 🏢 O Cenário (Desafio)
* **Cliente:** Distribuidora farmacêutica com operação on-premise no RJ.
* **Dor Principal:** Medo de expandir para o Sudeste devido ao alto custo de aquisição de servidores (CAPEX) e risco de paradas por quedas de energia.
* **Restrição:** Diretoria financeira com perfil conservador, exigindo ROI claro e alta segurança de dados fiscais/regulatórios.


## 🏗️ Arquitetura Proposta (Roadmap de Implementação)

A solução segue uma estratégia de **implementação em fases**, desenhada para gerar confiança gradual na diretoria e ROI imediato, conforme o AWS Well-Architected Framework.

### Fase 1: Armazenamento e Proteção de Ativos (Amazon S3)
* **Ação:** Migração imediata de backups e arquivos fiscais para a nuvem.
* **Recurso:** Implementação de *Object Lock* para proteção contra Ransomware e armazenamento de baixo custo para notas fiscais (NFe).
* **Ganho:** Segurança jurídica imediata e eliminação do risco de perda de dados por falha elétrica no Rio de Janeiro.

### Fase 2: Computação Elástica (Amazon EC2 + Auto Scaling)
* **Ação:** Migração do ERP e Sistema de Vendas.
* **Recurso:** Substituição do data center físico por instâncias virtuais que escalam automaticamente conforme a demanda de vendas (expansão Sudeste).
* **Ganho:** Redução de custos operacionais (OPEX) eliminando a ociosidade de servidores noturnos.

### Fase 3: Alta Disponibilidade e Resiliência (Amazon RDS Multi-AZ)
* **Ação:** Blindagem do Banco de Dados.
* **Recurso:** Banco de dados gerenciado com replicação síncrona em zonas de disponibilidade distintas (SP e redundância).
* **Ganho:** Continuidade de negócios garantida (Business Continuity) mesmo em cenários críticos de apagão na região primária.

## 📉 Comparativo Financeiro (CAPEX vs OPEX)

![On-Premise-vs-AWS-Cloud](/assets/On-Premise-vs-AWS-Cloud.png)


## 📂 Documentação do Projeto

* [📄 Relatório Completo de Implementação](./docs/relatorio-implementacao-aws.md)


## 🛠️ Skills Demonstradas
* Arquitetura de Soluções Cloud (AWS).
* Planejamento de Migração (Lift & Shift / Re-platform).
* Análise de Negócios (Business Case).
* Disaster Recovery (DR) e Continuidade de Negócios (BCP).

---
*Autor: [Seu Nome]*
