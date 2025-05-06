# [EN] Discord Giveaway Bot

A simple Discord bot for creating and managing giveaways in your server.

## Features

- Create giveaways with customizable duration, prize, and winner count
- End giveaways early
- Reroll winners for giveaways
- Simple permission system (requires Manage Messages permission)

## Setup

1. Clone this repository
2. Install dependencies:
   ```
   npm install
   ```
3. Create a `.env` file based on the `env.example` file:
   ```
   TOKEN=your_discord_bot_token
   PREFIX=!
   ```
4. Create a Discord bot and get your token:
   - Go to the [Discord Developer Portal](https://discord.com/developers/applications)
   - Create a new application
   - Go to the "Bot" tab and click "Add Bot"
   - Copy the token and add it to your `.env` file
   - Enable necessary Intents (Message Content, Server Members, etc.)

5. Invite the bot to your server:
   - Go to the "OAuth2" tab in the Developer Portal
   - Select "bot" under scopes
   - Select the following permissions:
     - Read Messages/View Channels
     - Send Messages
     - Manage Messages
     - Embed Links
     - Add Reactions
     - Read Message History
   - Copy the generated URL and open it in your browser to invite the bot

6. Start the bot:
   ```
   node index.js
   ```

## Commands

- `!giveaway [duration in minutes] [winners] [prize]` - Creates a new giveaway
- `!end [message ID]` - Ends a giveaway early
- `!reroll [message ID] [winners]` - Rerolls winners for an ended giveaway
- `!help` - Shows all available commands

## Examples

- `!giveaway 60 1 Discord Nitro` - Creates a 1-hour giveaway for Discord Nitro with 1 winner
- `!giveaway 1440 3 $10 Steam Gift Card` - Creates a 24-hour giveaway for a Steam Gift Card with 3 winners
- `!end 123456789012345678` - Ends the giveaway with the provided message ID
- `!reroll 123456789012345678 2` - Rerolls 2 winners for the giveaway with the provided message ID

## Required Permissions

Users need the "Manage Messages" permission to create, end, and reroll giveaways. 

# [PL] Bot Giveaway Discord

Prosty bot Discord do tworzenia i zarządzania giveaway w Twoim serwerze.

## Funkcje

- Tworzenie giveaway z konfigurowalnym czasem, nagrodą i liczbą zwycięzców
- Kończenie giveaway przed czasem
- Ponowne losowanie zwycięzców
- Prosty system uprawnień (wymaga uprawnienia do zarządzania wiadomościami)

## Ustawienia

1. Sklonuj to repozytorium
2. Zainstaluj zależności:
   ```
   npm install
   ```
3. Utwórz plik `.env` na podstawie pliku `env.example`:
   ```
   TOKEN=twój_token_bota_discord
   PREFIX=!
   ```
4. Utwórz bota Discord i zdobądź swój token:
   - Przejdź do [Portalu Dewelopera Discord](https://discord.com/developers/applications)
   - Utwórz nową aplikację
   - Przejdź do zakładki "Bot" i kliknij "Dodaj Bota"
   - Skopiuj token i dodaj go do swojego pliku `.env`
   - Włącz niezbędne intencje (Zawartość wiadomości, Członkowie serwera itp.)

5. Zaproś bota na swój serwer:
   - Przejdź do zakładki "OAuth2" w Portalu Dewelopera
   - Wybierz "bot" w zakresie
   - Wybierz następujące uprawnienia:
     - Odczyt wiadomości/Widok kanałów
     - Wysyłanie wiadomości
     - Zarządzanie wiadomościami
     - Osadzanie linków
     - Dodawanie reakcji
     - Odczyt historii wiadomości
   - Skopiuj wygenerowany URL i otwórz go w przeglądarce, aby zaprosić bota

6. Uruchom bota:
   ```
   node index.js
   ```

## Komendy

- `!giveaway [czas w minutach] [zwycięzcy] [nagroda]` - Tworzy nowy giveaway
- `!end [message ID]` - Kończy giveaway przed czasem
- `!reroll [message ID] [zwycięzcy]` - Ponownie losuje zwycięzców zakończonego giveaway
- `!help` - Pokazuje wszystkie dostępne komendy

## Przykłady

- `!giveaway 60 1 Discord Nitro` - Tworzy 1-godzinny giveaway z 1 zwycięzcą dla Discord Nitro
- `!giveaway 1440 3 $10 Steam Gift Card` - Tworzy 24-godzinny giveaway dla karty podarunkowej Steam z 3 zwycięzcami
- `!end 123456789012345678` - Kończy giveaway z podanym ID wiadomości
- `!reroll 123456789012345678 2` - Ponownie losuje 2 zwycięzców dla giveaway z podanym ID wiadomości

## Wymagane Uprawnienia

Użytkownicy muszą mieć uprawnienia "Zarządzanie wiadomościami", aby tworzyć, kończyć i ponownie losować giveaway.

