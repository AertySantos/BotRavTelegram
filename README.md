# Telegram Bot for Text Extraction

Este repositório contém o código-fonte de um bot do Telegram desenvolvido em Bash para receber mensagens de texto, extrair texto de imagens e também extrair texto de arquivos de áudio.

## Funcionalidades

### Recebimento de Mensagens de Texto
O bot está configurado para receber mensagens de texto simples enviadas pelos usuários. Ele pode processar qualquer tipo de texto, desde perguntas simples até comandos específicos.

### Extração de Texto de Imagens
Além de mensagens de texto, o bot pode receber imagens contendo texto. Utilizando tecnologias de reconhecimento óptico de caracteres (OCR), o bot é capaz de extrair o texto presente nas imagens e enviá-lo de volta ao usuário.

### Extração de Texto de Sons
Outra funcionalidade deste bot é a capacidade de extrair texto de arquivos de áudio. Utilizando tecnologias avançadas de reconhecimento de fala, o bot converte o áudio em texto e retorna o conteúdo ao usuário.

## Como Utilizar

1. **Configuração do Ambiente**
   - Clone este repositório em sua máquina local.

2. **Configuração do Bot no Telegram**
   - Crie um novo bot no Telegram utilizando o [BotFather](https://core.telegram.org/bots#botfather).
   - Copie o token fornecido pelo BotFather.

3. **Instalação das Dependências**
   - Certifique-se de ter o `curl`, `jr` e outras ferramentas de linha de comando necessárias instaladas em seu sistema.
   - sudo apt-get install jq
   - sudo apt-get install curl
   - sudo apt-get install tesseract-ocr
   - sudo apt-get install tesseract-ocr-por
   - sudo apt install ffmpeg
   - pip install SpeechRecognition
   - pip install pyaudio
   - Provavelmente dará algum erro
   - sudo apt-get install python3-pyaudio
   - sudo apt-get install portaudio19-dev python-all-dev python3-all-dev
   - pip install pyaudio
   - python -m speech_recognition

4. **Configuração das Credenciais**
   - Crie um arquivo `config.sh` na raiz do projeto.
   - Adicione suas credenciais ao arquivo `config.sh` da seguinte maneira:

    ```bash
    TELEGRAM_TOKEN="seu_token_aqui"

    ```

5. **Execução do Bot**
   - Execute `./main.sh` para iniciar o bot.

6. **Utilização no Telegram**
   - Encontre o bot no Telegram e inicie uma conversa.
   - Envie mensagens de texto, imagens ou arquivos de áudio para testar as funcionalidades de extração de texto.

## Contribuição
Contribuições são bem-vindas! Se você deseja melhorar este bot de alguma forma, sinta-se à vontade para enviar um pull request.
