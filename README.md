# Olá, eu sou o Henrique.

<img align="right" src="https://raw.githubusercontent.com/sindresorhus/sindresorhus/main/cat-typing.gif" width="110" alt="Gatinho digitando no computador" />

**Python · TypeScript · Automação · IA aplicada**

Sou estudante de **Análise e Desenvolvimento de Sistemas** e desenvolvo ferramentas com **Python e TypeScript**. Meu foco está em automação, integração de APIs e inteligência artificial aplicada a problemas concretos.

Também trabalho com **suporte técnico**. Investigar falhas, entender o que o usuário precisa e encontrar a causa de um problema fazem parte da minha rotina — e da forma como construo software.

## O que estou construindo

<a href="https://github.com/HenriquePvAr/Tradutor.Ia"><img src="./assets/yomu-architecture.svg" width="100%" alt="Yomu Sekai — aquisição, OCR, tradução, reconstrução e revisão em um pipeline orquestrado" /></a>

### Yomu Sekai · visão computacional, IA e linguagem

Desenvolvo um sistema de tradução de mangás, manhwas e webtoons que combina **visão computacional, inteligência artificial e processamento de linguagem natural (PLN)**. O pipeline localiza e reconhece textos com OCR, segmenta regiões com máscaras e usa inpainting para reconstruir as áreas após a remoção dos caracteres. Depois, traduz as falas, verifica a consistência dos termos e ajusta a tipografia aos balões, buscando preservar a composição artística original.

| Camada | Como funciona |
| :--- | :--- |
| **Interface e execução** | A UI grava jobs em uma fila SQLite. Um worker supervisionado executa cada job em um processo próprio e persiste progresso e resultados. |
| **Pipeline visual e linguístico** | Adapters coletam as páginas; RapidOCR identifica texto; a classificação contextual distingue falas, narração e SFX. A tradução passa por backend autenticado, com o motor remoto no servidor. |
| **Memória de capítulo** | Um ledger de terminologia e um registro de personagens mantêm nomes e formas canônicas consistentes dentro do capítulo. Cache e artefatos persistidos permitem reutilizar etapas válidas. |
| **Reconstrução e qualidade** | OpenCV, máscaras e inpainting apoiam a reconstrução; a análise geométrica orienta a posição e o tamanho da tradução. Verificações de resíduos de texto e alterações visuais registram evidências e encaminham casos duvidosos para revisão humana. |

**Python · OpenCV · RapidOCR · SQLite**<br>
Beta técnica em desenvolvimento. A fidelidade visual da reconstrução em páginas reais ainda está em validação.

[Explorar o Yomu →](https://github.com/HenriquePvAr/Tradutor.Ia) · [Arquitetura e processos](https://github.com/HenriquePvAr/Tradutor.Ia/blob/main/docs/technical/DOCUMENTACAO_TECNICA.md)

---

<a href="https://github.com/HenriquePvAr/Nodaris"><img src="./assets/nodaris-architecture.svg" width="100%" alt="Nodaris — Gateway MCP, agente local, projetos autorizados e núcleo de memória estruturada" /></a>

### Nodaris · contexto de projeto para assistentes de IA

Desenvolvo uma infraestrutura para conectar assistentes de IA a projetos locais com acesso controlado. Além de consultar arquivos, pesquisar código e inspecionar Git, o projeto tem um núcleo de memória estruturada para preservar o contexto do trabalho entre sessões: o que foi tentado, por que uma decisão foi tomada e quais evidências sustentam cada conclusão.

| Camada | Como funciona |
| :--- | :--- |
| **Gateway MCP + agente local** | O Gateway expõe as ferramentas aos clientes de IA; o agente valida cada solicitação e acessa somente as pastas autorizadas. Os processos se comunicam por HTTP autenticado e rodam em loopback por padrão. |
| **Registry e permissões** | O desenho de autorização vincula repositório, workspace e vault por identidade. Leitura, escrita de memória e escrita de projeto têm escopos próprios; uma não libera a outra. |
| **Núcleo de memória** | Vault Markdown como fonte de verdade, com missões, bugs, tentativas, decisões, experimentos, evidências e sessões relacionados por IDs. Histórico e resumos de continuidade distinguem relato, observação de teste e verificação Git. |
| **Escrita controlada** | O core separa proposta, aprovação e aplicação, com revisão esperada, hashes e recibos vinculados ao preview. A integração operacional depende dos gates locais de autorização, segurança e recuperação. |

**TypeScript · Node.js · MCP · Markdown / Obsidian**<br>
O runtime portátil publicado oferece leitura de projetos e Git. O núcleo de memória existe no repositório; sua habilitação no runtime portátil e a escrita em projetos continuam em desenvolvimento.

[Explorar o Nodaris →](https://github.com/HenriquePvAr/Nodaris) · [Arquitetura de memória](https://github.com/HenriquePvAr/Nodaris/blob/main/docs/architecture/NODARIS_MEMORY_BLUEPRINT.md)

## Por trás do código

Gosto de entender o caminho inteiro: da interface ao processamento, dos dados à decisão. É isso que me leva a trabalhar com automação, visão computacional e ferramentas para IA.

- **Investigar a causa.** Entender onde e por que algo falhou antes de escolher a correção.
- **Tornar o resultado verificável.** Registrar testes, decisões e limitações para poder avaliar o que foi construído.
- **Dar continuidade ao trabalho.** Organizar código e contexto para que a próxima etapa tenha uma base clara.

---

### Vamos trocar uma ideia?

Para conversar sobre os projetos, colaborar ou falar de uma oportunidade em desenvolvimento:

**[LinkedIn ↗](https://www.linkedin.com/in/henrique-paiva-14076a367) · [E-mail ↗](mailto:henriquepaiva128@gmail.com)**
