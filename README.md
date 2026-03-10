# Desafio QA Beedoo 2026

Análise e testes do módulo de cadastro e listagem de cursos.

**Aplicação:** https://creative-sherbet-a51eac.netlify.app/

---

## Objetivo da aplicação

Sistema para cadastro, listagem e exclusão de cursos educacionais, com suporte a dois tipos — presencial e online — cada um com campos específicos no formulário.



## Fluxos disponíveis

- **Cadastro de curso** — formulário com campos fixos (nome, descrição, instrutor, imagem, datas, vagas, tipo) e um campo condicional (endereço para presencial, link de inscrição para online)
- **Listagem de cursos** — exibição dos cursos cadastrados em cards com os dados registrados e imagem de capa
- **Exclusão de curso** — remoção de cursos a partir da listagem
- **Navegação** — alternância entre as telas pelo menu superior



## Pontos críticos para teste

- **Validação de campos obrigatórios** — o formulário não indica quais campos são obrigatórios, o que levantou a necessidade de verificar se o sistema impede cadastros incompletos
- **Consistência entre datas** — sem regra visível entre data de início e fim, era preciso validar se o sistema aceita intervalos incoerentes
- **Campo de vagas** — campo numérico com dois métodos de entrada (digitação e setas), ambos precisavam ser validados quanto a limites mínimos
- **Exclusão** — ação destrutiva que exige verificar se há confirmação prévia e se a remoção é efetiva
- **Campos condicionais** — comportamento dinâmico do formulário ao alternar entre tipos de curso
- **Formato de dados entre telas** — garantir que as informações cadastradas são exibidas de forma consistente na listagem

---

## Entregáveis

- **Cenários de teste, execução e bugs:** planilha https://docs.google.com/spreadsheets/d/1q0AENJj_kCia1kGFj76d5CgiCGP1fjEiOLZVfYKyuhU/edit?usp=sharing
- **Evidências de execução:** https://drive.google.com/drive/folders/1lX1wjJGeisp1VupfjbapDkb9K_Qg6I1X?usp=sharing
