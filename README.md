[![virtualLibraryAPI](https://github.com/danielso2007/projeto_checkstyle_pmd_jacoco/actions/workflows/maven-publish.yml/badge.svg)](https://github.com/danielso2007/projeto_checkstyle_pmd_jacoco/actions/workflows/maven-publish.yml)
[![codecov](https://codecov.io/gh/danielso2007/projeto_checkstyle_pmd_jacoco/branch/develop/graph/badge.svg)](https://codecov.io/gh/danielso2007/projeto_checkstyle_pmd_jacoco)
[![Quality Gate Status](https://sonarcloud.io/api/project_badges/measure?project=danielso2007_projeto_checkstyle_pmd_jacoco&metric=alert_status)](https://sonarcloud.io/summary/new_code?id=danielso2007_projeto_checkstyle_pmd_jacoco)
![GitHub package version](https://img.shields.io/github/package-json/v/danielso2007/projeto_checkstyle_pmd_jacoco.svg)
[![GitHub pull requests](https://img.shields.io/github/issues-pr-raw/danielso2007/projeto_checkstyle_pmd_jacoco.svg)](https://github.com/danielso2007/projeto_checkstyle_pmd_jacoco/pulls)
[![GitHub issues](https://img.shields.io/github/issues/danielso2007/projeto_checkstyle_pmd_jacoco.svg)](https://github.com/danielso2007/projeto_checkstyle_pmd_jacoco/issues?q=is%3Aopen+is%3Aissue)
![GitHub last commit](https://img.shields.io/github/last-commit/danielso2007/projeto_checkstyle_pmd_jacoco.svg)
[![GitHub issue/pull request author](https://img.shields.io/github/issues/detail/u/danielso2007/projeto_checkstyle_pmd_jacoco/1.svg)](https://github.com/danielso2007/projeto_checkstyle_pmd_jacoco/pulls)
![GitHub contributors](https://img.shields.io/github/contributors/danielso2007/projeto_checkstyle_pmd_jacoco.svg)
![GitHub top language](https://img.shields.io/github/languages/top/danielso2007/projeto_checkstyle_pmd_jacoco.svg)
[![GitHub All Releases](https://img.shields.io/github/downloads/danielso2007/projeto_checkstyle_pmd_jacoco/total.svg)](https://github.com/danielso2007/projeto_checkstyle_pmd_jacoco/archive/main.zip)
[![Conventional Commits](https://img.shields.io/badge/Conventional%20Commits-1.0.0-yellow.svg)](https://conventionalcommits.org)

<p align="center">
  <h3 align="center">Padr??es de projeto criacionais</h3>

  <p align="center">
    O objetivo desse projeto ?? apresentar as melhores ferramentas para ajudar programadores a seguir o melhro padr??o de um bom desenvolvimento de software.
    <br />
    <a href="https://github.com/danielso2007/projeto_checkstyle_pmd_jacoco"><strong>Explore the docs ??</strong></a>
    <br />
    <br />
    <a href="https://github.com/danielso2007/projeto_checkstyle_pmd_jacoco">View Demo</a>
    ??
    <a href="https://github.com/danielso2007/projeto_checkstyle_pmd_jacoco/issues">Report Bug</a>
    ??
    <a href="https://github.com/danielso2007/projeto_checkstyle_pmd_jacoco/issues">Request Feature</a>
  </p>
</p>


<!-- TABLE OF CONTENTS -->
<details open="open">
  <summary>Table of Contents</summary>
  <ol>
    <li>
      <a href="#checkstyle">Checkstyle</a>
      <ul>
        <li><a href="#caracter??sticas">Caracter??sticas</a></li>
        <li><a href="#o-arquivo-de-configura????o">O arquivo de configura????o</a></li>
        <li><a href="#executando-a-verifica????o-de-estilo-de-c??digo">Executando a verifica????o de estilo de c??digo</a></li>
      </ul>
    </li>
    <li>
      <a href="#configura????o-de-formata????o-e-clean-up-para-sts-e-eclipse">Configura????o de formata????o e clean up para STS e Eclipse</a>
    </li>
    <li>
      <a href="#pmd---analisador-de-c??digo-fonte-est??tico">PMD - Analisador de c??digo fonte est??tico</a>
      <ul>
        <li><a href="#executando-a-verifica????o-da-an??lise-est??tica-do-c??digo">Executando a verifica????o da an??lise est??tica do c??digo</a></li>
        <ul>
            <li><a href="#resultado-em-xml">Resultado em XML</a></li>
            <li><a href="#resultado-em-html">Resultado em HTML</a></li>
        </ul>
      </ul>
    </li>
    <li>
      <a href="#cobertura-de-c??digo">Cobertura de c??digo</a>
      <ul>
        <li><a href="#biblioteca-de-cobertura-de-c??digo-java-jaCoCo">Biblioteca de Cobertura de C??digo Java JaCoCo</a></li>
        <li><a href="#executando-a-cobertura-de-c??digo">Executando a cobertura de c??digo</a></li>
      </ul>
    </li>
  </ol>
</details>

## Checkstyle

Checkstyle ?? uma ferramenta de desenvolvimento para ajudar programadores a escrever c??digo Java que segue um padr??o de codifica????o. Ele automatiza o processo de verifica????o do c??digo Java para poupar os humanos dessa tarefa chata (mas importante). Isso o torna ideal para projetos que desejam impor um padr??o de codifica????o.

Checkstyle ?? altamente configur??vel e pode ser feito para suportar quase qualquer padr??o de codifica????o.

[Documenta????o do checkstyle, aqui.](https://checkstyle.sourceforge.io/)

### Caracter??sticas

Checkstyle pode verificar muitos aspectos do seu c??digo-fonte. Ele pode encontrar problemas de design de classe, problemas de design de m??todo. Ele tamb??m tem a capacidade de verificar o layout do c??digo e problemas de formata????o.

Para obter uma lista detalhada de checks dispon??veis, consulte a p??gina [checks](https://checkstyle.sourceforge.io/checks.html).

### O arquivo de configura????o

O arquivo de configura????o est?? nas pasta `config/checkstyle.xml`. A maior parte das configur????es segue o padr??o [Google Java Style](https://checkstyle.sourceforge.io/styleguides/google-java-style-20180523/javaguide.html).

### Executando a verifica????o de estilo de c??digo

Executar no terminal o comando:

```shell
mvn clean package checkstyle:check
```
Neste momento, no terminal, ser?? exibido as informa????es caso ocorra alguma viola????o. Tamb??m, na pasta `/target`, o resultado em `checkstyle-result.xml`.

## Configura????o de formata????o e clean up para STS e Eclipse

Na pasta `clean_up_formatter` h?? dois arquivos de formata????o que podem ser usados no Eclipse e STS para padronizar todas as formata????es de todas as classes do seu projeto, ganhando muito tempo nas corre????es dos estilos do c??digo.

## PMD - Analisador de c??digo fonte est??tico

PMD ?? um analisador de c??digo fonte est??tico. Ele encontra falhas de programa????o comuns, como vari??veis ??????n??o utilizadas, blocos catch vazios, cria????o desnecess??ria de objetos e assim por diante. Ele se preocupa principalmente com Java e Apex, mas suporta seis outras linguagens.

O PMD apresenta muitas verifica????es internas (no jarg??o do PMD, rules), que s??o documentadas para cada idioma em nossas [refer??ncias de regras](https://pmd.sourceforge.io/pmd-6.49.0/#shuffle-panel-rule-references). Tamb??m oferecemos suporte a uma API extensa para [escrever suas pr??prias regras](https://pmd.sourceforge.io/pmd-6.49.0/#shuffle-panel-writing-rules), que voc?? pode fazer em Java ou como uma consulta XPath independente.

 PMD ?? mais ??til quando integrado ao seu processo de compila????o . Ele pode ent??o ser usado como um port??o de qualidade, para impor um padr??o de codifica????o para sua base de c??digo. Entre outras coisas, o PMD pode ser executado:

 - Como uma [meta do Maven](https://pmd.sourceforge.io/pmd-6.49.0/pmd_userdocs_tools_maven.html)

### Executando a verifica????o da an??lise est??tica do c??digo

 Executar no terminal o comando:

```shell
mvn clean package pmd:check
```
Neste momento, no terminal, ser?? exibido as informa????es caso ocorra alguma viola????o. Tamb??m, na pasta `/target`, o resultado em `/site/pmd.html` e nas `pmd.xml`.

#### Resultado em XML

<p align="center">
    <img src="imgs/pmd_01.png" alt="Exemplo de resultado no XML" width="100%" height="100%">
</p>

#### Resultado em HTML

<p align="center">
    <img src="imgs/pmd_02.png" alt="Exemplo de resultado no HTML" width="100%" height="100%">
</p>

## Cobertura de c??digo

[EclEmma](https://www.eclemma.org/index.html) ?? uma ferramenta gratuita de cobertura de c??digo Java. Ele traz a an??lise de cobertura de c??digo diretamente para o ambiente de trabalho do Eclipse:

- **Ciclo de desenvolvimento/teste r??pido**: Lan??amentos de dentro do ambiente de trabalho, como execu????es de teste JUnit, podem ser analisados diretamente para cobertura de c??digo.
- **An??lise de cobertura avan??ada**: Os resultados da cobertura s??o imediatamente resumidos e destacados nos editores de c??digo-fonte Java.
- **N??o invasivo**: EclEmma n??o requer a modifica????o de seus projetos ou qualquer outra configura????o.
 
Desde a vers??o 2.0, o EclEmma ?? baseado na biblioteca de cobertura de c??digo JaCoCo. A integra????o do Eclipse tem seu foco no suporte ao desenvolvedor individual de uma forma altamente interativa. Para compila????es automatizadas, consulte a [documenta????o do JaCoCo](https://www.jacoco.org/jacoco/trunk/doc/) para [integra????es com outras ferramentas](https://www.jacoco.org/jacoco/trunk/doc/integrations.html).

### Biblioteca de Cobertura de C??digo Java JaCoCo

JaCoCo ?? uma biblioteca gratuita de cobertura de c??digo para Java, que foi criada pela equipe EclEmma com base nas li????es aprendidas com o uso e integra????o de bibliotecas existentes por muitos anos.

### Executando a cobertura de c??digo

O comando abaixo executar?? todas as verifica????es como PMD e checkstyle. ?? necess??rio que os testes tamb??m sejam executados junto com o `verify`. Caso seus testes estejam separados em um `profile`, execute junto com o `verify`.

```shell
mvn clean package verify
```
