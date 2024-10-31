# Sistema de Auxílio e Localização de Vítimas em Áreas Alagadas

Neste projeto, utilizamos o modelo YOLOv5, uma das arquiteturas de detecção de objetos mais avançadas, para identificar objetos específicos em imagens capturadas por drones. O objetivo é desenvolver um sistema capaz de automatizar a identificação de elementos como telhados e pessoas, proporcionando uma ferramenta útil para tarefas de monitoramento e inspeção aérea.

Este repositório contém um projeto que utiliza a ESP32-CAM para detecção de objetos, com foco em identificar vítimas em áreas alagadas. Abaixo, você encontrará uma breve descrição de cada arquivo e pasta incluídos.

## Estrutura do Repositório

- **best/**: Contém os arquivos gerados automaticamente após o treinamento do modelo YOLOv5.
- **images/**: Inclui as imagens utilizadas no treinamento do modelo, divididas em duas pastas:
  - **train**: Imagens de treino.
  - **val**: Imagens de validação.
- **labels/**: Contém as labels criadas para o modelo, utilizando ferramentas como [MakeSense](https://www.makesense.ai/) ou [Roboflow](https://roboflow.com/), divididas em:
  - **train**: Labels correspondentes às imagens de treino.
  - **val**: Labels correspondentes às imagens de validação.
- **print_epocas/**: Prints do treinamento do modelo, especificamente de cada época.
- **imgs_train_batch_colab/**: Imagens geradas para teste da detecção do modelo desenvolvido no Google Colab, sem a utilização da ESP32.
- **DetectObjects.ipynb**: Notebook Jupyter/Google Colab que contém o código para desenvolver o modelo `best.pt` usado no arquivo `MAIN.py`.
- **MAIN.py**: Código principal para trabalhar com a ESP32-CAM conectada à rede. Utiliza o modelo treinado (`best.pt`) para realizar a detecção de objetos.
- **best.pt**: Modelo treinado utilizado no script `MAIN.py`.
- **bibliotecas_esp32.zip**: Arquivo contendo as bibliotecas necessárias para executar a aplicação na ESP32-CAM.
- **telhado.yaml**: Arquivo de configuração contendo as definições das classes do modelo e os caminhos para os conjuntos de dados, utilizado no DetectObjects.ipynb.
- **sketch.ino**: Código gravado na ESP32-CAM para conectar à rede Wi-Fi e capturar imagens.
- **VIDEO.webm**: Vídeo de exemplo mostrando a aplicação do modelo para detecção de objetos.
- **README.md**: Este arquivo de descrição do projeto.

## Link para Demonstração

Assista ao teste da aplicação na ESP32-CAM no YouTube: [Link para o vídeo](https://youtu.be/H4tDFH1Y4Wo).

---

Este README fornece uma visão geral do repositório e seus arquivos, sem entrar em detalhes de como implementar o projeto do zero. Para saber mais ou replicar o projeto, sinta-se à vontade para explorar cada arquivo ou entrar em contato comigo através do GitHub.

---

## Projeto Acadêmico

PROJETO ACADÊMICO FIAP NEXT, COM PARTICIPAÇÃO DOS ALUNOS:
- Cristiano W. Dias
- Ana Carolina M. Silva
- Lucas Ichiama
- Santiago N. Bernardes

  
