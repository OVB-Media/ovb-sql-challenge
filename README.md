# SQL Challenge für Datenanalysten in unserem Medienunternehmen

## Einführung

Willkommen zur SQL-Challenge von OVB MEDIA! In der Medienbranche spielen Daten eine entscheidende Rolle bei der Verständigung über Nutzerverhalten, Inhaltsoptimierung und Abonnementwachstum. Deine Aufgabe wird es sein, anhand bereitgestellter Daten einige dieser Schlüsselfragen zu beantworten.

## Aufgabenstellung

Du hast einen Datensatz eines Medienunternehmens erhalten, der aus drei Tabellen besteht: `sessions`, `users`, und `subscriptions`. Deine Aufgabe ist es, das Nutzerverhalten und die Abonnementtrends zu analysieren:

1. **Aktive Nutzer:** Ermittle die Anzahl der einzigartigen Nutzer, die in den letzten 7 Tagen mindestens einmal auf die Plattform zugegriffen haben.
2. **Häufigste Inhalte:** Finde die Top 5 Artikel (basierend auf den Sessiondaten), die in den letzten 30 Tagen am häufigsten angesehen wurden.
3. **Abonnementkonvertierung:** Wie viele Nutzer, die sich in den letzten 6 Monaten registriert haben, haben innerhalb von 30 Tagen nach der Registrierung ein Abonnement abgeschlossen?

## Datenstruktur

### sessions Tabelle:
- `session_id` (unique identifier)
- `user_id` (foreign key to users table)
- `content_id` (ID des angesehenen Artikels/Videos)
- `session_start` (Startzeitpunkt der Session)
- `session_end` (Endzeitpunkt der Session)

### users Tabelle:
- `user_id` (unique identifier)
- `registration_date` (Datum der Nutzerregistrierung)

### subscriptions Tabelle:
- `subscription_id` (unique identifier)
- `user_id` (foreign key to users table)
- `subscription_start` (Startdatum des Abonnements)
- `subscription_end` (Enddatum des Abonnements, null wenn noch aktiv)

## Vorgehensweise und Abgabe

1. **Datenvorbereitung:** 
   - Nutze die gegebenen Datenstrukturen und Beispieldaten, um deine SQL-Abfragen zu formulieren und zu überprüfen.
2. **SQL-Abfragen testen:** 
   - Um die Genauigkeit deiner SQL-Abfragen sicherzustellen, kannst du bspw. [DB Fiddle](https://www.db-fiddle.com/) verwenden.
3. **Dateiorganisation:** 
   - Bitte erstelle für jede der drei gestellten Aufgaben eine separate `.sql` Datei. Die Dateinamen könnten beispielsweise `ActiveUsers.sql`, `TopContents.sql` und `SubscriptionConversion.sql` lauten.
4. **Einreichung:** 
   - Richte ein neues GitHub-Repository ein, in das du die drei `.sql` Dateien hochlädst. Sende uns den Link zu deinem GitHub-Repository an [karriere@ovbmedia.de](mailto:karriere@ovbmedia.de).
   - Alternativ kannst du die drei `.sql` Dateien an [karriere@ovbmedia.de](mailto:karriere@ovbmedia.de) senden.
