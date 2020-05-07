---
layout: project
type: project
image: images/socle-batch.png
title: SocleBatch
permalink: projects/socle-batch
# All dates must be YYYY-MM-DD format!
date: 2019-04-02
labels:
  - Spring-Batch
  - Spring
  - Java
summary: Une Api Json pour vos projets spring-batch avec des outils en plus.
---

[socle-batch](https://github.com/tisseurdetoile/socle-batch) Est un jeu d'outils pour ajouter une API JSON pour requêter vos application springbatch. A la manière de ce que faisait [spring-batch-admin](https://github.com/spring-attic/spring-batch-admin)(plus maintenu depuis 2017).

Le premier but est de fournir une API simple rétrocompatible avec **spring-batch-admin** le tout en étant sur des versions de spring et spring-batch plus récente.

Le deuxième but est de fournir des outils pour la manipulation des éléments courants pour les batch comme les fichiers COBOL (fichier à taille fixe) avec le [FixedLineTokenizerBuilder](https://github.com/tisseurdetoile/socle-batch/blob/master/springbatch-socle-tools/src/main/java/net/tisseurdetoile/batch/socle/tools/fixedlinetokenizer/FixedLineTokenizerBuilder.java) qui facilite la création du FixedLineTokenizer correspondant.

La mise en route est aussi simple que de rajouter ces librairies dans votre pom.xml

Pour l'API :

```xml
       <dependency>
           <groupId>net.tisseurdetoile.batch</groupId>
           <artifactId>springbatch-socle-jsonapi</artifactId>
           <version>0.2</version>
       </dependency>
```

Pour les outils :

```xml
     <dependency>
           <groupId>net.tisseurdetoile.batch</groupId>
           <artifactId>springbatch-socle-tools</artifactId>
           <version>0.2</version>
       </dependency>

```
