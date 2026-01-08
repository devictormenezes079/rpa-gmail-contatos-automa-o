# Automação RPA de Extração e Envio de Relatórios (Gmail)

Este projeto é uma automação de processos robóticos (RPA) desenvolvida em Python. O objetivo é simular o fluxo de trabalho de um usuário que precisa entrar em um sistema (neste caso, o Gmail), extrair um relatório de contatos, processar os dados e realizar o disparo automático de e-mails para a lista extraída.

## Funcionalidades

O script executa os seguintes passos:
1.  **Acesso ao Sistema:** Abre o Google Chrome e navega até o Gmail.
2.  **Navegação:** Localiza e clica nos menus de navegação para acessar a aba de Contatos.
3.  **Extração (Exportação):** Realiza a exportação dos contatos para um arquivo CSV.
4.  **Tratamento de Dados:** Utiliza a biblioteca `Pandas` para ler o arquivo baixado e limpar colunas vazias.
5.  **Automação de E-mail:** Percorre a lista de contatos e envia um e-mail personalizado para cada destinatário utilizando reconhecimento de imagem e comandos de teclado.

## Tecnologias Utilizadas

* [Python 3.13+](https://www.python.org/)
* [PyAutoGUI](https://pyautogui.readthedocs.io/): Para automação de interface gráfica (mouse e teclado).
* [Pandas](https://pandas.pydata.org/): Para manipulação e tratamento de dados do arquivo CSV.
* [Pyperclip](https://pypi.org/project/pyperclip/): Para lidar com a cópia de textos contendo caracteres especiais e acentuação.
* [OpenCV (opencv-python)](https://pypi.org/project/opencv-python/): Utilizado como suporte para o reconhecimento de imagem com precisão (`confidence`).

## Pré-requisitos

Antes de rodar o script, você precisará instalar as dependências necessárias:


pip install pyautogui pandas opencv-python pyperclip