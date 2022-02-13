# Projekt Adjuvant

[![GitHub issues](https://img.shields.io/github/issues/projekt-adjuvant/adjuvant)](https://github.com/projekt-adjuvant/adjuvant/issues)
[![GitHub license](https://img.shields.io/github/license/projekt-adjuvant/adjuvant)](https://github.com/projekt-adjuvant/adjuvant)

Ein Amazon Alexa Plugin zur Unterstützung von Patienten mit Demenz bei der Einhaltung von Terminen und der Berechnung von Routen.

## Inhalte

- [**Beschreibung**](#-beschreibung)
- [**Konfiguration**](#-konfiguration)
- [**Technologie**](#-technologie)
- [**Dokumente**](#-dokumente)
- [**Fehler gefunden?**](#-fehler-gefunden)
- [**Urheberrecht**](#urheberrecht)

## 📋 Beschreibung

**Hinweis:** Momentan handelt es sich bei Adjuvant um einen Prototypen!

Der Prototyp läuft auf der Plattform [Amazon Alexa](https://developer.amazon.com/alexa) und anstehende Termine des Patienten werden in der Cloud gespeichert. Dafür wird die NoSQL-Datenbank [AWS DynamoDB](https://www.aws.com/dynamodb) verwendet und der Programmcode (Java) wird in [AWS Lambda](https://www.aws.com/lambda) ausgeführt.

Darüber hinaus wurden die [GeoCode Routing API](https://geocode.dev.stefan.zone/github) und ein zugehöriges [Java SDK](https://geocode.dev.stefan.zone/java/sdk) entwickelt, das ebenfalls als Package im [Maven Central Repository](https://search.maven.org/artifact/zone.stefan.dev/geocode/1.0.1/jar) verfügbar ist. Es bietet einen einfachen Zugriff auf die berechneten Routendaten in Java, die von der REST-API zurückgegeben werden.

Die Entwicklung erfolgte agil mit Scrum, so dass das Feedback der Betroffenen und ihrer Angehörigen inkrementell eingearbeitet werden konnte. Um Werkzeuge wie [JUnit](https://junit.org/), [Jacoco](https://www.jacoco.org/jacoco/) und [Checkstyle](https://checkstyle.org/) vollständig automatisiert ausführen zu können, wurde zudem eine [Gitlab CI/CD](https://docs.gitlab.com/ee/ci/) Pipeline ([`.gitlab-ci.yml`](../../blob/main/.gitlab-ci.yml)) konfiguriert.

## ⚙️ Konfiguration

Um Adjuvant verwenden zu können, wird ein [Entwickler Konto](https://developer.amazon.com/alexa/console/signin) für Amazon Alexa benötigt. Befindet sich das Projekt in der `development` Phase, so muss jedes Projektmitglied als Entwickler eingeladen werden.

Zur Konfiguration können die Dateien im Ordner ([`.alexa`](../../blob/main/.alexa)) verwendet werden. Sie ermöglichen jederzeit Adjuvant von Grund auf neu aufzusetzen.

## 🔨 Technologie

Bei der Entwicklung wurden folgende Technologien und Werkzeuge eingesetzt.

- **Code**: [Java](https://www.java.com)
- **Datenbank**: [AWS DynamoDB](https://www.aws.com/dynamodb)
- **Rechner**: [AWS Lambda](https://www.aws.com/lambda)
- **CI/CD**: [Gitlab CI](https://docs.gitlab.com/ee/ci/)

## 📃 Dokumente

- **Pressemitteilung**: [Hier klicken](https://files.stefan.zone/software-engineering/documents/press_release.pdf)
- **Projektpräsentation**: [Hier klicken](https://files.stefan.zone/software-engineering/documents/product_presentation.pdf)

## 👷‍ Fehler gefunden?

Vielen Dank für Ihre Nachricht! Bitte füllen Sie einen [Fehlerbericht](../../issues/new?assignees=&labels=&template=bug_report.yaml&title=) aus. Wir werden uns dann so schnell wie möglich um eine Lösung bemühen.

## Urheberrecht

&copy; 2020 – 2022 Projekt Adjuvant, Alle Rechte vorbehalten.
