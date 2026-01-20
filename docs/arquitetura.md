# Diagrama de Arquitetura – Operação Farmacêutica

## Visão Geral
A arquitetura proposta utiliza serviços serverless da AWS para reduzir custos operacionais e permitir escalabilidade automática para a operação farmacêutica.

## Fluxo da Arquitetura

Farmácias Parceiras  
→ Amazon API Gateway  
→ AWS Lambda (Regras de Negócio)  
→ Amazon SNS (Evento: Pedido Criado)  
→ Amazon DynamoDB (Pedidos e Produtos)  
→ Amazon S3 (Notas Fiscais e Relatórios)

## Objetivo
Eliminar servidores físicos, reduzir custos iniciais e permitir crescimento conforme a entrada de novas farmácias parceiras.
