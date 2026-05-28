# AgSUS - COGIP

<Adicionar objetivo da organização, missão e etc>

---

## Criação de Repositórios e Governança

Para garantir que todos os novos projetos sigam as diretrizes de qualidade da organização, **não criamos repositórios manualmente**. Utilizamos uma esteira automatizada que padroniza a estrutura inicial de qualquer código.

### Workflow: `Policy for creation of repository`
Sempre que precisar iniciar um novo projeto na organização, acesse a aba **Actions** e execute o workflow de criação preenchendo os seguintes campos:

* **Nome do projeto:** O nome do sistema ou componente.
* **Visibilidade:** Definição se o projeto será `público` ou `privado`.
* **Descrição:** Resumo do objetivo do repositório.

---

## O que a automação faz?

Assim que executada, a ferramenta cria o repositório do zero e injeta uma série de boas práticas essenciais:

* **Nomenclatura Padronizada:** Alinha o nome do projeto com as regras da organização, aplicando automaticamente o prefixo oficial (`COGIP_`) e limpando espaços ou caracteres especiais.
* **Mensagens de Commit Monitoradas:** Configura travas locais para garantir que todo o time utilize o padrão internacional de **Conventional Commits** (como `feat:`, `fix:`, `chore:`), mantendo o histórico de alterações limpo e legível. *(A instrução de ativação é adicionada automaticamente ao README do repositório gerado).*
* **Formulários de Issues Estruturados:** Configura formulários interativos em substituição aos textos livres. O repositório já nasce preparado com moldes específicos para **Relato de Bug**, **Nova Funcionalidade**, **Melhoria de Documentação** e **Dúvida/Suporte**.
* **Template de Pull Request:** Cria um padrão para a união de códigos com tabelas de evidências (antes vs. depois), vinculação automática de tarefas e checklists de qualidade (Definition of Done) antes da aprovação.
* **Proteção de Branches (Rulesets):** Caso o projeto seja público, o robô ativa regras automáticas para proteger a branch principal (`main`), exigindo a aprovação de pelo menos um revisor e proibindo a exclusão acidental da branch.
* **Sistema de Rollback:** Se por algum motivo o repositório for criado mas a injeção das políticas de qualidade falhar, a esteira apaga o repositório automaticamente para evitar projetos incompletos ou fora das normas da COGIP.

---
