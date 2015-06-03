# DSL "Logic" für die dialogische Logik

Domänen-spezifische Sprache für die dialogische Logik.

**Dateiendung:** .logic
**Grammatikname:** Logic

# Build

Eclipse -> Settings -> Git -> Projects -> Automatically ignore derived resources .. UNCHECK

## Generierung des DSL-Editors als RCP Anwendung



# Grammatik

## Grundlegende Grammatik für logische Aussagen

Verzicht auf Negation. Ausdruck durch natürliche Sprache, für Auswertung nicht notwendig, da sowieso ein menschlicher Akteur die Aussage auf sic, non oder non-liquet bewerten muss.

Umfang der Grammatik:

- Konjunktion
- Adjunktion 
- Subjunktion (Implikation)
- Einsquantor (Existenzquantor)
- Allquantor

### Konkrete Syntax

Assozivität: Von links nach rechts gelten die Vorrangsregeln. Andernfalls muss mit «» geklammert werden.

Jedes Keyword (und, oder etc.) sind innerhalb der Elemtaraussage nicht erlaubt.

Der Punkt . begrenzt einzelne Aussagen.

- Aussage= «aussage» und|oder etc. «aussage».
- Elementaraussage= «elementaraussage»
- Konjunktion= «elementaraussage» und «elementaraussage»
- Adjunktion= «elementaraussage» oder «elementaraussage»
- Subjunktion (Implikation)= wenn|es gilt «elementaraussage» deshalb|darauf folgt|darum|daher|dann «elementaraussage»
- Einsquantor (Existenzquantor)= für mindestens einen|ein|eine «beliebiger text» gilt: «elementaraussage».
- Allquantor= für alle «beliebiger text» gilt: «elementaraussage». 

