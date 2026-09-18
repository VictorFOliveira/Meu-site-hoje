# 🌵 Cactus Tecnologia

Site institucional da Cactus Tecnologia e portal de entrada para o ecossistema de soluções SaaS.

## Produtos iniciais
- **Cactus Food** — gestão de restaurantes, bares e lanchonetes
- **Cactus Gestão** — gestão de academias
- **Cactus Fight** — gestão de academias de luta
- **Cactus Ponto** — controle de ponto e jornada
- **Minha Escola** — SaaS de gestão escolar, acadêmica e administrativa

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


### Privacidade e infraestrutura

A apresentação do Cactus Ponto também acompanha a evolução técnica do produto:

- centro de privacidade para o titular, com exportação dos próprios dados e fluxo de solicitações;
- controles de segurança e isolamento multi-tenant;
- PostgreSQL como fonte de verdade;
- Redis como camada de cache e rate limit distribuído, com fallback para manter disponibilidade;
- domínio por empresa, branding por tenant e suporte a domínio próprio.

O site evita alegar certificação ou conformidade jurídica automática; os exemplos representam funcionalidades técnicas do produto.


## Demonstração do Minha Escola

O card **Minha Escola** abre uma apresentação interativa dentro do portfólio, sem obrigar o visitante a sair do site.

A prévia apresenta oito experiências integradas do SaaS:

- **Administração / Coordenação** — matrículas, turmas, grade curricular e estrutura acadêmica;
- **Portal do Aluno** — notas, médias, horários, professores, frequência e acompanhamento formativo;
- **Diário do Professor** — aula por disciplina, conteúdo ministrado, tarefa, observações e chamada;
- **Avaliações** — provas, trabalhos, pesos, lançamento de notas e média parcial;
- **Financeiro / Responsável** — mensalidades, bolsas, pagamentos, boletins e gateway opcional;
- **Comunicação** — avisos, leitura, ciência, anexos e autorizações;
- **Secretaria / Documentos** — declarações, boletins, históricos e recibos verificáveis;
- **Superadmin** — tenants, planos, assinaturas, onboarding e auditoria.

### Estrutura atual do produto

O Minha Escola chegou à versão 1.0 com as 11 fases planejadas implementadas e já possui:

- autenticação e autorização por perfil;
- contas de aluno vinculadas diretamente à matrícula;
- contas de professor vinculadas ao cadastro docente;
- responsáveis vinculados aos próprios alunos;
- matrículas e rematrículas com histórico;
- disciplinas, períodos, grade curricular e quadro de horários;
- avaliações, notas, pesos e médias parciais;
- acompanhamento formativo com controle de visibilidade;
- diário do professor;
- frequência por disciplina e por aula;
- política acadêmica configurável;
- fechamento de médias por período;
- boletim oficial;
- recuperação;
- média final e resultado da matrícula;
- planos e contratos financeiros por matrícula;
- bolsas e descontos;
- mensalidades, baixa e inadimplência;
- Asaas opcional e sistema externo compatível;
- Portal do Responsável com boletins e pagamentos;
- comunicação por público e autorizações;
- alertas acadêmicos e financeiros;
- documentos com snapshot e código de verificação;
- onboarding de escola;
- planos e assinaturas SaaS;
- Superadmin separado;
- limites por plano;
- auditoria e exportação de dados;
- job diário e health/readiness da aplicação.

As telas exibidas no portfólio são previews demonstrativos coerentes com a arquitetura e os fluxos implementados no repositório **Minha-escola**.


### Estado de implantação

A base funcional das 11 fases está no repositório **Minha-escola**. Uma publicação comercial real ainda depende da infraestrutura escolhida para produção, como banco PostgreSQL gerenciado, domínio, TLS, backups, observabilidade e credenciais dos provedores opcionais.
