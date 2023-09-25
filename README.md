# Slack Bot voor Dagelijkse Berichten

Dit project bevat een Slack bot die automatisch een bericht post in een Slack-kanaal op een specifieke tijd.

## Vereisten

- Python 3.x
- Een Slack API token

## Installatie en Configuratie

1. **Kloon de Repository**  
   ```
   git clone https://github.com/jouw-gebruikersnaam/jouw-repository.git
   ```

2. **Installeer de Benodigdheden**  
   Ga naar de map van het project en voer de volgende commando's uit:
   ```
   pip install -r requirements.txt
   ```

3. **Configuratie van Slack API Token**
   - Maak een Slack app via de Slack API Console en verkrijg een API token met de `chat:write` scope.
   - Voeg het token toe aan een `.env`-bestand in de root van het project met de volgende indeling:
     ```
     SLACK_API_TOKEN=jouw-token-hier
     ```

4. **GitHub Secrets**
   - Ga naar de GitHub-pagina van jouw repository, navigeer naar "Settings" -> "Secrets" en voeg het Slack API token toe met de naam `SLACK_API_TOKEN`.

## Gebruik

Het script kan direct worden uitgevoerd voor een eenmalige post, of het kan worden gescheduled via GitHub Actions.

1. **Direct Gebruik**  
   ```
   python app.py
   ```

2. **Gebruik via GitHub Actions**  
   - Configureer het `.github/workflows/main.yml`-bestand om het script op een bepaalde tijd uit te voeren.
   - Voor meer informatie over het instellen van de workflow, zie [deze link](#).
