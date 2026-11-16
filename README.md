# Henrique Paiva

## 01 · Apresentação

**Desenvolvedor de software | Python, TypeScript e sistemas com IA**

Construo ferramentas que integram inteligência artificial, automação e infraestrutura de software. Atualmente desenvolvo o **Komyst**, para processamento visual de capítulos ilustrados, e o **Nodaris**, que conecta assistentes de IA a projetos locais autorizados.

Estudo Análise e Desenvolvimento de Sistemas e trabalho com suporte técnico. Investigar problemas e transformá-los em soluções práticas faz parte do meu dia a dia.

## 02 · Projetos em destaque

### Komyst

Aplicativo para processar e traduzir capítulos ilustrados, combinando visão computacional, tradução por backend autenticado e reconstrução de imagens.

- Recebe fontes compatíveis ou arquivos locais e organiza o processamento em uma fila persistente, com worker separado.
- Usa RapidOCR e classificação para localizar e interpretar texto antes da tradução.
- Reconstrói as páginas e gera os arquivos escolhidos; resultados que precisam de inspeção ficam marcados para revisão.

<p align="center">
  <img src="./assets/komyst-nova-traducao.png" width="100%" alt="Tela Komyst para iniciar uma tradução, escolher a origem e acompanhar as etapas do processamento" />
</p>

**Estado:** beta técnica; fidelidade visual e casos sinalizados ainda exigem validação e revisão. [Repositório](https://github.com/HenriquePvAr/Komyst) · [Problemas conhecidos](https://github.com/HenriquePvAr/Komyst/blob/main/docs/KNOWN_ISSUES.md)

### Nodaris

Infraestrutura MCP que permite a assistentes consultar projetos locais aprovados.

`Assistente de IA → cliente MCP → Gateway local → agente local → projeto autorizado`

- O operador seleciona as pastas permitidas; o runtime local protege sua configuração e mantém o Gateway em loopback por padrão.
- Disponibiliza leitura de arquivos, pesquisa de código e inspeção Git nos projetos autorizados.
- O runtime portátil atual é somente leitura; escrita em memória ou nos projetos não está habilitada nele.

[Repositório](https://github.com/HenriquePvAr/Nodaris) · [Instalação em outro computador](https://github.com/HenriquePvAr/Nodaris/blob/main/docs/guides/INSTALLATION_NEW_PC.md)

## 03 · Tecnologias e práticas

**Komyst:** Python · OpenCV · RapidOCR · SQLite

**Nodaris:** TypeScript · Node.js · MCP

**Engenharia:** workers isolados · APIs autenticadas · permissões explícitas · testes e revisão de qualidade

Os READMEs dos projetos descrevem as validações executadas e os limites atuais de cada versão.

## 04 · Atividade e contato

Estudante de ADS e profissional de suporte técnico. Aberto a conversar sobre IA aplicada, automação, ferramentas de desenvolvimento e oportunidades.

[LinkedIn](https://www.linkedin.com/in/henrique-paiva-14076a367) · [E-mail](mailto:henriquepaiva128@gmail.com)
