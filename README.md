# Bash AI Cli

Command-line script to interact with AI models quickly and easily.

## 🚀 Installation

1. Install the script:
```bash
# Create Scripts directory if it doesn't exist
mkdir -p $HOME/Scripts && cd $HOME/Scripts

# Download the script directly to Scripts
git clone https://github.com/chelo91/bash-ai-cli.git ./
chmod +x ai
```

2. Configure the variables file:
```bash
# Create configuration file
touch .config

# Edit the file with your preferred editor (example with nano)
nano .config
```

3. Add these variables to the `.config` file:
```bash
API_KEY="your-api-key"
PROMPT="instructions-for-ai"
API_URL="api-url"
MODEL="model-to-use"
```

4. Make the command available globally:

For bash (add to the end of `~/.bashrc`):
```bash
echo 'export PATH="$HOME/Scripts:$PATH"' >> ~/.bashrc
source ~/.bashrc
```

For zsh (add to the end of `~/.zshrc`):
```bash
echo 'export PATH="$HOME/Scripts:$PATH"' >> ~/.zshrc
source ~/.zshrc
```

## 📝 Usage

El script puede ser usado de varias formas:

### 1. Consulta directa
Realiza una pregunta directamente desde la línea de comandos:
```bash
ai How do I create a directory in Linux

ai Explain this code: < mycode.js
```

### 2. Usando pipe (|)
Envía el contenido de un archivo o comando como contexto:
```bash
cat myfile.txt | ai What does this code do

ls -la | ai Explain these files

```

## ⚙️ Requirements

- Git
- bash or zsh
- curl
- jq

## 🤝 Contributing

Contributions are welcome. Please open an issue or pull request.