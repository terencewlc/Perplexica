Getting Started with Docker (Recommended)
Ensure Docker is installed and running on your system.

Clone the Perplexica repository:

git clone https://github.com/ItzCrazyKns/Perplexica.git
After cloning, navigate to the directory containing the project files.

Rename the sample.config.toml file to config.toml. For Docker setups, you need only fill in the following fields:

OPENAI: Your OpenAI API key. You only need to fill this if you wish to use OpenAI's models.

OLLAMA: Your Ollama API URL. You should enter it as http://host.docker.internal:PORT_NUMBER. If you installed Ollama on port 11434, use http://host.docker.internal:11434. For other ports, adjust accordingly. You need to fill this if you wish to use Ollama's models instead of OpenAI's.

GROQ: Your Groq API key. You only need to fill this if you wish to use Groq's hosted models.

ANTHROPIC: Your Anthropic API key. You only need to fill this if you wish to use Anthropic models.

Note: You can change these after starting Perplexica from the settings dialog.

SIMILARITY_MEASURE: The similarity measure to use (This is filled by default; you can leave it as is if you are unsure about it.)

Ensure you are in the directory containing the docker-compose.yaml file and execute:

docker compose up -d
Wait a few minutes for the setup to complete. You can access Perplexica at http://localhost:3000 in your web browser.

Note: After the containers are built, you can start Perplexica directly from Docker without having to open a terminal.

ollama
![ollama setup](https://github.com/user-attachments/assets/28b428d3-e392-4cec-bf71-45e9bff01386)

glm4flash
![glm-v4 setup](https://github.com/user-attachments/assets/4045adca-97dc-4488-9306-5f69368b7ea4)
