# Amazon RDS

O Amazon RDS (Relational Database Service) é um serviço gerenciado da AWS que facilita a criação, operação e escalabilidade de bancos de dados relacionais na nuvem.

💡 O que ele faz?

- O RDS cuida automaticamente de tarefas administrativas como:
- Provisionamento de hardware
- Instalação e configuração do banco
- Backups automáticos
- Patches de segurança
- Monitoramento e métricas
- Replicação e alta disponibilidade (Multi-AZ)

🗄️ Bancos de dados suportados

O Amazon RDS suporta vários mecanismos de banco de dados como: MySQL, PostgreSQL, Oracle, Microsoft SQL Server e Amazon Aurora (compatível com MySQL e PostgreSQL)

🚀 Benefícios principais

- Gerenciamento simplificado
  > Você não precisa cuidar do servidor nem de tarefas operacionais complexas.
- Escalabilidade
  > É fácil aumentar capacidade de CPU, memória ou armazenamento.
- Alta disponibilidade e recuperação de desastres
  > Configurações Multi-AZ e snapshots facilitam a resiliência.
- Desempenho otimizado
  > Com opções como armazenamento SSD e replicação de leitura.

📌 Quando usar o RDS?

Ele é ideal quando você precisa de um banco de dados relacional (SQL) sem querer gerenciar a infraestrutura por conta própria.


# Estratégias de Backup e Recuperação de Dados na AWS

Investir em estratégias de backup e recuperação na AWS é essencial para:

✔ Garantir a proteção dos dados
✔ Cumprir regulações
✔ Minimizar tempo de inatividade
✔ Aumentar a resiliência do negócio
✔ Reduzir custos e riscos
✔ Garantir operações contínuas e seguras

⚖️ Diferença entre estratégias

As estratégias de backup garantem cópias seguras e acessíveis dos dados. Já as estratégias de recuperação definem como restaurar a operação após incidentes, variando entre custo e velocidade.

🔹 Principais Estratégias de Backup
Backups automáticos: Uso de serviços como AWS Backup, RDS Automated Backups e EBS Snapshots para criar rotinas automáticas.
Versionamento: S3 Versioning para manter várias versões de um objeto.
Backups multi-região: Replicar dados para outra região para proteção contra falhas regionais.
Backup híbrido: Integração entre ambientes on-premises e AWS via AWS Storage Gateway.
Backup por camadas: Uso de S3 Glacier / Glacier Deep Archive para dados de longo prazo.

🔹 Princiapis Estratégias de Recuperação
Backup and Restore: Recuperação manual usando backups armazenados. Menor custo, maior tempo de recuperação.
Pilot Light: Apenas serviços essenciais rodando em outra região, ligados rapidamente em caso de falha.
Warm Standby: Ambiente reduzido sempre ativo e pronto para ser ampliado.
Multi-Region Active-Active: Todo o sistema funcionando em múltiplas regiões simultaneamente. Maior resiliência, maior custo.

<h3> ⭐ Boas Práticas de Backup e Recuperação </h3>


- Automatize as políticas de backup.
- Utilize taggings.
- Defina políticas de retenção.
- Use criptografa e segurança de acessos.
- Testar rotinas de recuperação regularmente.
- Faça monitoramento e auditoria.

