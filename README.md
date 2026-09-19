# 🌵 Cactus Tecnologia

Site institucional da Cactus Tecnologia e portal de entrada para o ecossistema de soluções SaaS.

## Produtos iniciais
- **Cactus Food** — gestão de restaurantes, bares e lanchonetes
- **Minha Academia** — SaaS multi-tenant para gestão de academias
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


## Demonstração do Minha Academia

O card **Minha Academia** substitui o antigo placeholder Cactus Gestão e agora abre uma demonstração interativa no próprio portfólio.

A apresentação acompanha a fundação funcional do repositório **Minha-academia** e mostra:

- dashboard operacional;
- cadastro e situação de alunos;
- planos e matrículas;
- turmas e grade recorrente;
- presença/check-in;
- cobranças, pagamentos e resumo financeiro;
- isolamento multi-tenant;
- RBAC server-side para OWNER, ADMIN, MANAGER, RECEPTION, COACH, FINANCE e STUDENT;
- base preparada para integrações futuras de pagamento e controle de acesso.

O preview evita anunciar como concluídos os módulos que ainda estão no roadmap, como ficha de treino, avaliação física, portal do aluno, Asaas, catracas, Wellhub e TotalPass.

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

O Minha Escola está em **release candidate para homologação final**, com as 11 fases planejadas implementadas. O dashboard autenticado já usa dados reais por tenant e a suíte técnica passou por regressão destrutiva concorrente. O produto já possui:

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

### Validação técnica atual

Em 18/09/2026, o passe final de regressão destrutiva do Minha Escola foi concluído com:

- 5.000 alunos;
- 3.000 cobranças;
- 44 usuários concorrentes;
- 2.000 requisições sustentadas com concorrência 100;
- 1.000 requisições em rajada com concorrência 250;
- dashboard SSR, Portal do Aluno e Portal do Responsável no mix;
- 3.000/3.000 respostas bem-sucedidas;
- 0 falhas e 0% de erro;
- readiness e migration status verdes após a carga;
- CI, CodeQL, dependency audit e validações de produção verdes.

O resultado é um baseline de CI e não substitui a homologação final na VPS/infraestrutura contratada.


### Estado de implantação

A base funcional e os gates automáticos estão fechados no repositório **Minha-escola**. O estado atual é **pronto para homologação final**. Uma publicação comercial real ainda depende da infraestrutura escolhida para produção, como VPS/containers, PostgreSQL, domínio, TLS, storage/scanner, backups, observabilidade, secrets e credenciais dos provedores opcionais.
