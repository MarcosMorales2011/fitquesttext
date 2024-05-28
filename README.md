# FitQuest Discord Bot

## Overview

FitQuest is a Discord bot that enhances your fitness journey by integrating RPG elements into your daily workouts. Users can join or create parties to explore dungeons, complete daily quests, and earn rewards. The bot supports both free and premium features, providing an engaging experience for all users.

## Features

### Free Features
- **Dungeon Raids/Joining Parties**: Explore dungeons, encounter enemies, and progress through quests.
- **Joining Guilds**: Join guilds, participate in guild activities, and earn exclusive rewards.
- **Daily Quests/Bounties**: Complete daily quests and bounties to gain experience points (XP).
- **Viewing Character Sheet**: View detailed character sheets, including attributes and cosmetic items.

### Premium Features
- **Additional Life**: Extra life during dungeon raids.
- **Special Dungeons**: Access harder dungeons with greater rewards.
- **Special Cosmetic Items**: Exclusive cosmetic items for premium users.
- **Boss Rush**: Challenge strong bosses for additional rewards.
- **Creating Guilds/Parties**: Premium users can create guilds and parties.

## Getting Started

### Prerequisites
- Python 3.7+
- Discord account and a server to add the bot to
- Discord bot token (create one [here](https://discord.com/developers/applications))

### Installation

1. Clone the repository:
    ```sh
    git clone https://github.com/yourusername/FitQuest-Discord-Bot.git
    cd FitQuest-Discord-Bot
    ```

2. Create and activate a virtual environment:
    ```sh
    python -m venv venv
    source venv/bin/activate  # On Windows use `venv\Scripts\activate`
    ```

3. Install the required dependencies:
    ```sh
    pip install -r requirements.txt
    ```

4. Set up the configuration:
    - Copy `config/config.example.yaml` to `config/config.yaml` and fill in the required values, including your Discord bot token.

### Running the Bot

Start the bot using the following command:
```sh
python src/bot.py
```

## Project Structure

```plaintext
FitQuest-Discord-Bot/
├── README.md
├── requirements.txt
├── .gitignore
├── config/
│   ├── config.yaml
│   └── logging.yaml
├── src/
│   ├── __init__.py
│   ├── bot.py
│   ├── commands/
│   │   ├── __init__.py
│   │   ├── admin_commands.py
│   │   ├── free_user_commands.py
│   │   ├── premium_user_commands.py
│   └── events/
│       ├── __init__.py
│       ├── event_handlers.py
│       ├── dungeon_events.py
│       └── guild_events.py
├── data/
│   ├── __init__.py
│   ├── database.py
│   ├── models/
│   │   ├── __init__.py
│   │   ├── character.py
│   │   ├── guild.py
│   │   └── dungeon.py
│   └── repositories/
│       ├── __init__.py
│       ├── character_repo.py
│       ├── guild_repo.py
│       └── dungeon_repo.py
├── utils/
│   ├── __init__.py
│   ├── data_loader.py
│   ├── embed_builder.py
│   ├── command_utils.py
│   └── validation.py
├── tests/
│   ├── __init__.py
│   ├── test_bot.py
│   ├── test_commands/
│   │   ├── __init__.py
│   │   ├── test_admin_commands.py
│   │   ├── test_free_user_commands.py
│   │   └── test_premium_user_commands.py
│   ├── test_events/
│   │   ├── __init__.py
│   │   ├── test_event_handlers.py
│   │   ├── test_dungeon_events.py
│   │   └── test_guild_events.py
│   ├── test_data/
│   │   ├── __init__.py
│   │   ├── test_database.py
│   │   ├── test_character_repo.py
│   │   ├── test_guild_repo.py
│   │   └── test_dungeon_repo.py
│   └── test_utils/
│       ├── __init__.py
│       ├── test_data_loader.py
│       ├── test_embed_builder.py
│       ├── test_command_utils.py
│       └── test_validation.py
└── docs/
    ├── architecture.md
    ├── api_reference.md
    └── user_guide.md
```

## Configuration

### config.yaml
Configure your bot settings in the `config/config.yaml` file. This includes your bot token, prefixes for commands, and other relevant settings.

### logging.yaml
Set up logging configurations in the `config/logging.yaml` file to manage log levels and output formats.

## Contributing

We welcome contributions from the community. If you'd like to contribute, please follow these steps:

1. Fork the repository.
2. Create a new branch (`git checkout -b feature/your-feature-name`).
3. Commit your changes (`git commit -m 'Add some feature'`).
4. Push to the branch (`git push origin feature/your-feature-name`).
5. Open a pull request.

## License

This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.

## Contact

For any questions or support, please contact Marcos Morales at marcosmorales2011@gmail.com

---

This README file provides a comprehensive overview and guide to setting up and contributing to the FitQuest Discord Bot project.