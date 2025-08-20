# RELATÓRIO DE IMPLEMENTAÇÃO DE SERVIÇOS AWS

**Data:** 19/08/2025  
**Empresa:** Abstergo Industries  
**Responsável:** Daniel Martins de Andrade  

---

## Introdução

Este relatório descreve o processo de implementação de ferramentas de computação em nuvem na **Abstergo Industries**, uma distribuidora farmacêutica que atua como elo entre fabricantes e farmácias responsáveis pelo atendimento ao consumidor final. O trabalho foi conduzido por **Daniel Martins de Andrade**.

Atualmente, a empresa não utiliza nenhuma solução em nuvem, o que resulta em altos custos com infraestrutura física, gastos recorrentes de manutenção e limitações operacionais. A iniciativa surgiu a partir de uma conversa com o gestor financeiro, que demonstrou interesse em avaliar como a adoção da **cloud computing** poderia reduzir custos e, ao mesmo tempo, aumentar a eficiência dos processos internos. 

Sendo um hub de distribuição farmacêutica, a Abstergo lida diariamente com grandes volumes de dados, integração com parceiros estratégicos e a necessidade de alta confiabilidade em seus serviços.

Nesse contexto, a migração para a **AWS Cloud** surge como uma solução estratégica, oferecendo ganhos em escalabilidade, segurança e otimização de custos. Além disso, possibilita que a empresa concentre mais recursos no crescimento do negócio. Para iniciar esse processo, foram selecionados três serviços da AWS com alto potencial de impacto positivo e retorno rápido.

---

## Descrição do Projeto

O projeto foi estruturado em **3 etapas principais**, cada uma com foco em um aspecto essencial para a redução de custos e aumento da eficiência operacional.

---

### Etapa 1
**Nome da ferramenta:** Amazon S3 (Simple Storage Service)  
**Foco da ferramenta:** Armazenamento seguro e econômico de documentos e arquivos.  

**Descrição de caso de uso:**  
Atualmente, a empresa mantém documentos (pedidos, notas fiscais, bulas, relatórios médicos e contratos) em servidores físicos locais, o que gera custos de:  
- Compra e atualização de hardware.  
- Espaço físico e energia elétrica.  
- Backup manual e gerenciamento de dados.  

Com a migração para o **Amazon S3**, esses custos são eliminados, pois o armazenamento passa a ser **pago por uso** (sem necessidade de compra de servidores). Além disso:  
- Políticas de ciclo de vida podem transferir documentos antigos automaticamente para camadas de menor custo, como **S3 Glacier**, gerando até 80% de economia em arquivos pouco acessados.  
- Alta durabilidade (99,999999999% - “11 noves”) garante que os documentos da Abstergo fiquem seguros, sem necessidade de manter cópias físicas.  
- Redução de riscos de perda de dados, que poderiam gerar custos regulatórios e jurídicos no setor farmacêutico.  

**Principal ganho:**  
Eliminação de custos fixos com servidores físicos e armazenamento escalável sob demanda, pagando apenas pelo que for utilizado.  

---

### Etapa 2
**Nome da ferramenta:** Amazon RDS (Relational Database Service)  
**Foco da ferramenta:** Banco de dados gerenciado com alta disponibilidade e baixo custo de manutenção.  

**Descrição de caso de uso:**  
Hoje a Abstergo mantém bancos de dados locais para controle de fornecedores, pedidos, estoques e clientes. Isso exige:  
- Licenciamento de software de banco de dados.  
- Hardware dedicado (servidores).  
- Equipe especializada para backup, manutenção e atualização.  

Ao migrar para o **Amazon RDS**, esses custos diminuem porque:  
- O banco de dados passa a ser totalmente gerenciado pela AWS (incluindo atualizações, backups automáticos, replicação e segurança).  
- A empresa paga apenas pelo uso (modelo *pay-as-you-go*), sem investir em servidores caros.  
- O sistema é escalável: nos períodos de maior demanda (ex.: lançamento de novos medicamentos ou campanhas promocionais), é possível aumentar a capacidade rapidamente e reduzir em seguida, sem custo extra de infraestrutura ociosa.  
- Disponibilidade garantida em múltiplas zonas de disponibilidade (alta resiliência contra falhas).  

**Principal ganho:**  
Redução de custos com licenciamento, manutenção e hardware, além de maior confiabilidade para dados críticos de estoque e pedidos.  

---

### Etapa 3
**Nome da ferramenta:** AWS Cost Explorer + AWS Budgets  
**Foco da ferramenta:** Controle e otimização de custos em tempo real.  

**Descrição de caso de uso:**  
Uma preocupação comum ao adotar cloud é a falta de visibilidade sobre os gastos. Para garantir que a Abstergo mantenha controle financeiro rígido, serão implementados os serviços **Cost Explorer** e **Budgets**, que permitem:  
- Monitorar em tempo real quais serviços estão consumindo mais recursos.  
- Definir alertas de orçamento: se os custos ultrapassam um valor definido, o gestor financeiro recebe uma notificação.  
- Criar relatórios detalhados por setor, permitindo identificar quais áreas da empresa consomem mais recursos de TI.  
- Identificar oportunidades de economia, sugerindo planos de instância reservada ou ajustes de uso.  

**Principal ganho:**  
Transparência total nos gastos com cloud e previsibilidade financeira, evitando surpresas na fatura e permitindo tomadas de decisão rápidas.  

---

## Conclusão

A implementação de ferramentas na empresa **Abstergo Industries** tem como esperado:  
- Redução de custos imediatos com armazenamento (Amazon S3) e banco de dados (Amazon RDS).  
- Eliminação da necessidade de servidores físicos, reduzindo custos com energia elétrica, manutenção e espaço físico.  
- Maior previsibilidade financeira por meio do AWS Cost Explorer e Budgets.  
- Escalabilidade automática, permitindo atender picos de demanda sem gastos fixos adicionais.  
- Segurança e compliance alinhados às exigências do setor farmacêutico.  

Com esses serviços, a Abstergo terá uma operação de TI mais enxuta, segura e flexível, liberando recursos financeiros que podem ser direcionados para **inovação, expansão comercial e aumento de competitividade no mercado farmacêutico**.  

---

## Anexos
- [AWS Documentation](https://docs.aws.amazon.com/)  

---

**Assinatura do Responsável pelo Projeto:**  

**Daniel Martins de Andrade**  
