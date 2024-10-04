# RELATÓRIO DE IMPLEMENTAÇÃO DE SERVIÇOS AWS

Data: 04 de outubro de 2024  
Empresa: Abstergo Industries  
Responsável: Giancarlo Castro  

## Introdução
Este relatório apresenta o processo de implementação de ferramentas na empresa Abstergo Industries, realizado por Giancarlo Castro. O objetivo do projeto foi elencar 3 serviços AWS, com a finalidade de realizar diminuição de custos imediatos.

## Descrição do Projeto
O projeto de implementação de ferramentas foi dividido em 3 etapas, cada uma com seus objetivos específicos. A seguir, serão descritas as etapas do projeto:

### Etapa 1:
- **Amazon EC2 (Elastic Compute Cloud) com instâncias spot**
- **Foco:** Redução de custos em servidores virtuais
- **Descrição de caso de uso:** 
  A empresa utilizava instâncias on-demand para hospedar suas operações de redistribuição e controle de inventário, o que resultava em custos elevados, especialmente em horários de pico. A proposta foi substituir parte das instâncias on-demand por instâncias spot, que são mais baratas e ideais para cargas de trabalho que podem ser interrompidas e retomadas, como relatórios de inventário e processos de análises periódicas.

### Etapa 2:
- **Amazon S3 (Simple Storage Service) com políticas de ciclo de vida**
- **Foco:** Otimização de armazenamento de dados
- **Descrição de caso de uso:** 
  A empresa armazenava grandes quantidades de dados históricos sobre remessas, pedidos e relatórios, muitos dos quais não eram acessados frequentemente, mas permaneciam em camadas de armazenamento mais caras. Foi implementada uma política de ciclo de vida no Amazon S3, que movimenta automaticamente os dados inativos para camadas de armazenamento de menor custo, como S3 Glacier, após um determinado período, resultando em economias significativas no custo de armazenamento.

### Etapa 3:
- **AWS Lambda**
- **Foco:** Redução de custos com infraestrutura por meio de computação serverless
- **Descrição de caso de uso:** 
  Muitas das operações de processamento de pedidos e validação de inventário ocorrem de forma intermitente e não requerem a execução constante de servidores dedicados. A utilização do AWS Lambda permitiu executar funções específicas sob demanda, eliminando a necessidade de servidores dedicados para tarefas simples e ocasionais. Isso reduziu a necessidade de manter servidores continuamente ativos, diminuindo os custos de operação.

## Conclusão
A implementação de ferramentas na empresa Abstergo Industries tem como esperado a redução de custos operacionais com servidores, armazenamento e processamento de dados, além do aumento da eficiência e produtividade por meio do uso de soluções escaláveis e automatizadas. Recomenda-se a continuidade da utilização das ferramentas implementadas e a busca por novas tecnologias que possam melhorar ainda mais os processos da empresa.

## Anexos
- [Relatório de custos pré e pós-implementação](https://aws.amazon.com/pricing/)
- [Guia de políticas de ciclo de vida no Amazon S3](https://docs.aws.amazon.com/AmazonS3/latest/userguide/lifecycle-configuration-examples.html)
- [Manual de boas práticas para o uso de AWS Lambda](https://docs.aws.amazon.com/lambda/latest/dg/best-practices.html)

Assinatura do Responsável pelo Projeto:  
Giancarlo Castro
