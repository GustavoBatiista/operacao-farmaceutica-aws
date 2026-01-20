# RELATÓRIO DE IMPLEMENTAÇÃO DE SERVIÇOS AWS

Data: 19/01/2026  
Empresa: Abstergo Industries  
Responsável: Gustavo de Oliveira Batista

---

## Introdução

Este relatório apresenta o processo de implementação de ferramentas na empresa Abstergo Industries, realizado por Gustavo de Oliveira Batista.  
O objetivo do projeto foi elencar 5 serviços da AWS, com a finalidade de promover redução imediata de custos, escalabilidade automática e modernização da infraestrutura, considerando que a empresa não possuía ambiente em cloud.

---

## Descrição do Projeto

O projeto de implementação de ferramentas foi dividido em 5 etapas, cada uma com seus objetivos específicos. A seguir, são descritas as etapas do projeto:


### Etapa 1:
- **Nome da ferramenta:** Amazon API Gateway  
- **Foco da ferramenta:** Gerenciamento e exposição de APIs  
- **Descrição de caso de uso:**  
  O Amazon API Gateway foi utilizado como ponto de entrada do sistema do "hub" farmacêutico, permitindo que farmácias parceiras realizem requisições para criação de pedidos e consulta de produtos. O uso desse serviço elimina a necessidade de servidores dedicados para receber requisições, reduzindo custos operacionais e oferecendo escalabilidade automática.


### Etapa 2:
- **Nome da ferramenta:** AWS Lambda  
- **Foco da ferramenta:** Execução de lógica de negócio sem servidores  
- **Descrição de caso de uso:**  
  A AWS Lambda foi utilizada para processar as regras de negócio do sistema, como validação de pedidos, cálculo de valores e geração de eventos. Por ser um serviço serverless, a empresa passa a pagar apenas pelo tempo de execução das funções, evitando custos com infraestrutura ociosa.


### Etapa 3:
- **Nome da ferramenta:** Amazon SNS  
- **Foco da ferramenta:** Comunicação assíncrona baseada em eventos  
- **Descrição de caso de uso:**  
  O Amazon SNS foi utilizado para publicar eventos de negócio, como a criação de pedidos. Esses eventos podem ser consumidos por diferentes serviços, como faturamento e notificações, de forma desacoplada. Essa abordagem reduz a complexidade de integrações diretas e facilita a expansão do sistema com baixo custo.


### Etapa 4:
- **Nome da ferramenta:** Amazon DynamoDB  
- **Foco da ferramenta:** Armazenamento de dados escalável e gerenciado  
- **Descrição de caso de uso:**  
  O Amazon DynamoDB foi adotado para armazenar dados de pedidos, produtos e farmácias parceiras. O serviço opera em modelo sob demanda, eliminando a necessidade de gerenciamento de servidores de banco de dados e permitindo que a empresa pague apenas pelas operações realizadas.


### Etapa 5:
- **Nome da ferramenta:** Amazon S3  
- **Foco da ferramenta:** Armazenamento de arquivos e documentos  
- **Descrição de caso de uso:**  
  O Amazon S3 foi utilizado para armazenar documentos do sistema, como notas fiscais, relatórios e contratos das farmácias parceiras. Trata-se de um serviço de armazenamento de baixo custo, alta durabilidade e cobrança baseada apenas no volume de dados armazenado.


## Conclusão

A implementação das ferramentas na empresa **Abstergo Industries** tem como resultado esperado a redução significativa de custos operacionais, aliada à escalabilidade e simplicidade de gerenciamento da infraestrutura.  
O uso de serviços serverless e gerenciados permite que a empresa atue como um hub farmacêutico sem a necessidade de investimentos elevados em infraestrutura física, pagando apenas pelo uso real dos recursos.  
Recomenda-se a continuidade da utilização das ferramentas implementadas e a avaliação constante de novas tecnologias que possam otimizar ainda mais os processos da empresa.



Assinatura do Responsável pelo Projeto:

Gustavo de Oliveira Batista
