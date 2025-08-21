# Relatório de Implementação de Serviços AWS
📅 Data: 21/08/2025  
🏢 Empresa:Abstergo Industries  
👩‍💻 Responsável: Melissa Martins  

---

## 📖 Introdução
Este documento apresenta o processo de implementação inicial de serviços da AWS na **FarmaTech Solutions**, realizado por **Melissa Martins**.  

A empresa, que até então utilizava apenas infraestrutura **on-premises**, buscava soluções em nuvem para:  

- 📉 Reduzir custos operacionais e de manutenção de datacenter  
- ⚡ Garantir **alta disponibilidade** dos sistemas críticos de pesquisa e vendas  
- 🔒 Melhorar a **segurança e conformidade regulatória** (LGPD e normas do setor farmacêutico)  
- 🚀 Modernizar a arquitetura de TI para suportar **análises de dados e escalabilidade**  

O projeto concentrou-se em três serviços essenciais da AWS: **Amazon EC2, Amazon S3 e Amazon RDS**.  

---

## 🛠️ Descrição do Projeto
O projeto foi dividido em três etapas, cada uma com foco na substituição de componentes críticos da infraestrutura local por soluções em nuvem, garantindo **economia, escalabilidade, segurança e simplicidade de manutenção**.  

---

### Etapa 1 — Computação em Nuvem
💻 **Serviço:** Amazon EC2  
🎯 **Objetivo:** Substituir servidores físicos por instâncias virtuais escaláveis para rodar aplicações críticas de gestão farmacêutica.  

📌 **Caso de uso:**  
- Os servidores locais que hospedavam o **ERP farmacêutico e sistemas de controle de estoque** geravam custos elevados com energia, refrigeração e manutenção.  
- Migração para instâncias **otimizadas para custo e performance** (ex.: t4g.medium e m5.large).  
- Configuração de **Auto Scaling** para atender picos de acesso em períodos de fechamento fiscal e auditorias regulatórias.  
- Implementação de **agendamento de desligamento automático** fora do horário comercial, reduzindo custos.  

---

### Etapa 2 — Armazenamento Escalável e Seguro
🗄️ **Serviço:** Amazon S3  
🎯 **Objetivo:** Centralizar, proteger e manter a conformidade dos arquivos corporativos.  

📌 **Caso de uso:**  
- Documentos de pesquisa, relatórios de qualidade e backups eram armazenados em servidores locais sujeitos a falhas.  
- Migração para o **Amazon S3**, garantindo **alta durabilidade (11 9’s)** e controle de acesso refinado via **IAM e políticas de bucket**.  
- Configuração de **S3 Intelligent-Tiering**, permitindo economia automática de custos sem impacto no desempenho.  
- Implementação de ciclo de vida para arquivamento em **S3 Glacier Instant Retrieval**, atendendo requisitos legais de retenção de documentos.  

---

### Etapa 3 — Banco de Dados Gerenciado
🗃️ **Serviço:** Amazon RDS  
🎯 **Objetivo:** Garantir alta disponibilidade, escalabilidade e segurança dos bancos de dados de clientes, estoque e pesquisas clínicas.  

📌 **Caso de uso:**  
- O banco de dados local exigia manutenção manual e não tinha redundância, apresentando risco para os dados sensíveis de pacientes e fornecedores.  
- Migração para o **Amazon RDS for PostgreSQL** com:  
  - **Multi-AZ** para alta disponibilidade  
  - **Backups automáticos e snapshots manuais**  
  - **Escalabilidade vertical sob demanda** para grandes consultas em relatórios  
  - **Criptografia em repouso e em trânsito**, atendendo normas de compliance da área farmacêutica  

---

## ✅ Conclusão
A implementação dos serviços **EC2, S3 e RDS** trouxe para a FarmaTech Solutions:  

- 💰 **Redução de custos** com servidores locais e licenciamento  
- 🔒 **Segurança e conformidade** no armazenamento e manipulação de dados sensíveis  
- ⚡ **Alta confiabilidade** dos sistemas críticos de estoque e clientes  
- 📊 Maior **flexibilidade para análises de dados** e auditorias  

📌 **Próximos passos sugeridos:**  
- Monitoramento contínuo com **Amazon CloudWatch**  
- Backup centralizado e políticas de recuperação com **AWS Backup**  
- Automação de tarefas de rotina com **AWS Lambda**  
- Implementação de **Amazon QuickSight** para relatórios e dashboards em tempo real  

---

## 📎 Anexos
🔗 [Amazon EC2](https://aws.amazon.com/ec2/)  
🔗 [Amazon S3](https://aws.amazon.com/s3/)  
🔗 [Amazon RDS](https://aws.amazon.com/rds/)  

---

✍️ **Assinatura:** Melissa Martins  
