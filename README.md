# 🌵 Cactus Tecnologia

Site institucional da Cactus Tecnologia e portal de entrada para o ecossistema de soluções SaaS.

## Produtos iniciais
- **Cactus Food** — gestão de restaurantes, bares e lanchonetes
- **Cactus Gestão** — gestão de academias
- **Cactus Fight** — gestão de academias de luta
- **Cactus Ponto** — controle de ponto e jornada

## Stack
React + TypeScript + Vite.

## Desenvolvimento
```bash
npm install
npm run dev
```

## Build
```bash
npm run build
```

A arquitetura comercial prevista é multi-tenant/white-label, com os produtos podendo compartilhar a infraestrutura central da Cactus e evoluir para serviços separados conforme a necessidade de escala.

## Demonstração do Cactus Ponto

A página institucional já apresenta exemplos visuais das duas experiências do produto:

- **/ponto** — portal do colaborador, com nome, logo e cores do tenant, jornada guiada e assinatura discreta "Desenvolvido por Cactus Tecnologia";
- **/admin** — central administrativa para ADMIN/RH/Gestor, com indicadores, equipe, ajustes e fechamento;
- domínio por empresa no padrão `empresa.ponto.cactustecnologia.com.br`, com suporte planejado/implementado para domínio próprio do cliente.

Os exemplos são demonstrativos e acompanham o comportamento atual do repositório Cactus Ponto.
