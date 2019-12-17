# Boas práticas

Este é um repositório de um arquivo só apenas para acordar sobre nossas boas práticas. Nossas do Núcleo de Computação Científica e Geoprocessamento (NCCG) - Instituto de Pesquisas Jardim Botânico do Rio de Janeiro.

Fundamentados em ciência aberta, somos um laboratório que usa controle de versão em git de todo seu fluxo de trabalho, independentemente da linguagem de programação utilizada. O material de desenvolvimento do pacote e ferramentas correlatas está [aqui](https://github.com/Model-R) e o material do Projeto Conservação e Restauração da Bacia Hidrográfica do Rio Doce (INMA/PCI), [aqui](https://github.com/Projeto-BHRD-INMA). 

Existem muitos bons materiais básicos de como usar o git, destacamos a página da [Jenny Bryan](https://happygitwithr.com/), o material básico de configuração do git no RStudio da [Page Picinini](https://pagepiccinini.com/r-course/lesson-0-introduction-and-set-up/), o material do [software carpentry](https://swcarpentry.github.io/git-novice/). Nada substitui o estudo e a prática.

Este não é um tutorial ou manual de como usar o git, apenas um acordo de boas práticas para adotarmos em nossos projetos.

## Dicas gerais

+ O git não é uma nuvem para backup de arquivos
+ Controlar versão de arquivos de texto apenas (texto simples ou código)
+ **SEMPRE** incluir um README.md na raiz do repositório
+ **SEMPRE** que possível incluir um README.md dentro de cara diretório no repositório
+ Usar o arquivo .gitignore para que o git ignore arquivos que não serão controlados e existem só localmente no seu computador

## Sobre a estrutura de pastas

Cara repositório tem sua estrutura específica, mas de modo geral adotamos a seguinte organização:

+ README.md descrição informativa do repositório. Deve citar fonte de dados
+ `data` para armazenar arquivos de dados, podem livremente ser organizados em subdiretórios
+ `R` ou `code` (ou o nome da extensão do arquivo da linguagem de programação que você usa) para armazenar arquivos de código. Separar os códigos por grande tarefa utilizada e nomeá-los usando número com dois dígitos e a tarefa, por exemplo: `01_download_dos_dados.R`
+ `results` para armazenar outputs gerados pelos códigos. Nomear os arquivos com a numeração referente ao script que o gerou, por exemplo: `01_lista_de_especies.R`
+ `figures` se necessário, para armazenar figuras geradas pelos códigos. Nomear os arquivos com a numeração referente ao script que o gerou, por exemplo: `01_mapa_especies_bacia.png`
+ `docs` se necessário, para guardar arquivos de texto versionáveis (.txt, .tex, .md, .Rmd) com textos e relatórios referentes ao projeto do repositório

**IMPORTANTE**: é de muito bom tom incluir um README.md dentro de cada diretório criado explicando os arquivos nele contido e/ou tarefas realizadas

