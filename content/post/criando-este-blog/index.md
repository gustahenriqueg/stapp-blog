---
title: Criando este blog - o making-of
description: Como decidi documentar minha jornada como DevOps/SRE construindo este blog em etapas, publicando primeiro e automatizando depois.
slug: criando-este-blog
date: 2026-07-12 10:00:00+0000
#image: cover.jpg
categories:
    - Azure
    - DevOps
tags:
    - Hugo
    - Azure
    - Terraform
    - GitHub Actions
#weight: 1
---

Trabalho como DevOps/SRE, com Azure, Terraform e Kubernetes no dia a dia. Depois de um tempo estudando e certificando (AZ-900, AZ-305), decidi que precisava de um lugar para organizar o que estou aprendendo — e nada melhor do que aplicar na prática o que pratico no trabalho: construir algo do zero, em etapas, documentando o caminho.

## Por que um blog, e por que assim

A tentação inicial era simples: já provisionar tudo com Terraform, já montar pipeline completo, já deixar "pronto" antes de publicar qualquer coisa. Só que isso é exatamente a receita para abandonar um projeto pessoal na metade — tentar entregar a versão perfeita antes de ter algo funcionando de verdade.

Então decidi inverter a lógica: publicar primeiro, automatizar depois, transformar em código por último. Cada etapa só avança quando a anterior já está de pé.

## As etapas até aqui

1. **Hugo local** — gerar o site estático com o tema [Stack](https://github.com/CaiJimmy/hugo-theme-stack), sem me preocupar ainda com infraestrutura.
2. **GitHub** — versionar o código do zero, mesmo antes de qualquer deploy.
3. **Azure Static Web Apps** — publicar manualmente via portal/CLI, sem Terraform, só para ver o blog no ar.
4. **GitHub Actions** — o próprio Azure já gerou um workflow de deploy ao criar o Static Web App; agora é revisar e entender esse pipeline em vez de escrever do zero.

## O que vem a seguir

- Explorar a Azure CLI para pequenas automações antes de ir para Terraform.
- Provisionar a infraestrutura como código, importando o que já existe hoje (em vez de recriar do zero).
- Domínio próprio, HTTPS e observabilidade básica.
- Mais adiante, comparar a experiência com Bicep, só por curiosidade técnica.

Este post é o marco zero. A ideia é voltar aqui e linkar os próximos posts técnicos conforme cada etapa avançar — Terraform, pipelines, Kubernetes, e o que mais surgir pelo caminho.