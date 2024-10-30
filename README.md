<h1 align="center">🧠 Sistema de Verificação de Identidade para Aplicações Bancárias</h1>
<br>

![Banner](https://github-dbrazl.s3.us-east-1.amazonaws.com/ai-face-recognition/banner.svg?)

<p align="center">
  Trabalho de Conclusão de Curso apresentado para obtenção do título de especialista em Inteligência Artificial e Aprendizado de Máquina – Pontifícia Universidade Católica de Minas Gerais (PUC Minas) – 2022.
</p>

<br>
<p align="center">
  <img src="https://img.shields.io/badge/autor-@dbrazl-blue?style=flat" alt="Autor: @dbrazl">
</p>
<br>

## 📝 Resumo

<p align="justify">
  Este trabalho apresenta o desenvolvimento de um sistema de verificação de identidade voltado para aplicações bancárias, utilizando uma rede neural convolucional para análise facial. Com o crescente uso de serviços bancários digitais, as instituições financeiras necessitam de mecanismos de segurança eficientes para prevenir fraudes. A solução proposta visa identificar o usuário durante transações bancárias, confirmando sua identidade por meio de reconhecimento facial. Para a realização da prova de conceito, foi coletado um conjunto de imagens de voluntários, que foi tratado e dividido para treinamento e validação do modelo. Utilizando a plataforma Colab e a biblioteca FastAI, foi possível treinar uma rede neural que obteve uma acurácia de 100% em uma base de teste reduzida. Os resultados indicam o potencial da aplicação para auxiliar na segurança de transações bancárias, minimizando o risco de fraudes.
</p>

## 🛠 Tecnologias

<p align="justify">
  As tecnologias utilizadas nesse projeto foram:
</p>

![Python](https://img.shields.io/badge/Python-333333?style=flat&logo=python&logoColor=green)
![Pandas](https://img.shields.io/badge/Pandas-333333?style=flat&logo=pandas&logoColor=blue)
![Numpy](https://img.shields.io/badge/Numpy-333333?style=flat&logo=numpy&logoColor=lightblue)
![Scikit-learn](https://img.shields.io/badge/-Scikit%2d-learn-333333?style=flat&logo=scikitlearn)
![Matplotlib](https://img.shields.io/badge/-Matplotlib-333333?style=flat&logo=data:image/svg+xml;base64,PD94bWwgdmVyc2lvbj0iMS4wIiBlbmNvZGluZz0iVVRGLTgiPz4KPHN2ZyB4bWxucz0iaHR0cDovL3d3dy53My5vcmcvMjAwMC9zdmciIHdpZHRoPSIxODAiIGhlaWdodD0iMTgwIiBzdHJva2U9ImdyYXkiPgo8ZyBzdHJva2Utd2lkdGg9IjIiIGZpbGw9IiNGRkYiPgo8Y2lyY2xlIGN4PSI5MCIgY3k9IjkwIiByPSI4OCIvPgo8Y2lyY2xlIGN4PSI5MCIgY3k9IjkwIiByPSI2NiIvPgo8Y2lyY2xlIGN4PSI5MCIgY3k9IjkwIiByPSI0NCIvPgo8Y2lyY2xlIGN4PSI5MCIgY3k9IjkwIiByPSIyMiIvPgo8cGF0aCBkPSJtOTAsMnYxNzZtNjItMjYtMTI0LTEyNG0xMjQsMC0xMjQsMTI0bTE1MC02MkgyIi8+CjwvZz48ZyBvcGFjaXR5PSIuOCI+CjxwYXRoIGZpbGw9IiM0NEMiIGQ9Im05MCw5MGgxOGExOCwxOCAwIDAsMCAwLTV6Ii8+CjxwYXRoIGZpbGw9IiNCQzMiIGQ9Im05MCw5MCAzNC00M2E1NSw1NSAwIDAsMC0xNS04eiIvPgo8cGF0aCBmaWxsPSIjRDkzIiBkPSJtOTAsOTAtMTYtNzJhNzQsNzQgMCAwLDAtMzEsMTV6Ii8+CjxwYXRoIGZpbGw9IiNEQjMiIGQ9Im05MCw5MC01OC0yOGE2NSw2NSAwIDAsMC01LDM5eiIvPgo8cGF0aCBmaWxsPSIjM0JCIiBkPSJtOTAsOTAtMzMsMTZhMzcsMzcgMCAwLDAgMiw1eiIvPgo8cGF0aCBmaWxsPSIjM0M5IiBkPSJtOTAsOTAtMTAsNDVhNDYsNDYgMCAwLDAgMTgsMHoiLz4KPHBhdGggZmlsbD0iI0Q3MyIgZD0ibTkwLDkwIDQ2LDU4YTc0LDc0IDAgMCwwIDEyLTEyeiIvPgo8L2c+PC9zdmc+)
![FastAI](https://img.shields.io/badge/FastAI-333333?style=flat&logo=data:image/svg+xml;base64,PHN2ZyB4bWxucz0iaHR0cDovL3d3dy53My5vcmcvMjAwMC9zdmciIHdpZHRoPSIxODAiIGhlaWdodD0iMTgwIiB2ZXJzaW9uPSIxLjAiIHZpZXdCb3g9IjAgMCAxMzUgMTM1Ij48cGF0aCBkPSJNOTAuODUgMzEuOTQzVjE0LjY5Nmg1MS43NDFWNDkuMTloLTUxLjc0Wk05Mi4wNjUgNzguNzA0VjY4LjEzOGgzNS43MDhWODkuMjdIOTIuMDY1Wk03MC42ODggMjIuNTkxdi03Ljg5NWgxNS43OXYxNS43OWgtMTUuNzl6TTcwLjY4OCA0My4zNnYtNy4yODdoMTUuNzl2MTQuNTc1aC0xNS43OXpNNTMuNDQxIDIyLjU5MXYtNy44OTVoMTQuMzMydjE1Ljc5SDUzLjQ0MXpNNTMuNDQxIDYxLjMzNnYtNy43NzNoMTQuMzMydjE1LjU0Nkg1My40NDF6TTM0LjczNyA0My4zNnYtNy4yODdoMTUuNzg5djE0LjU3NUgzNC43Mzd6TTUzLjQ0MSA4MS45ODR2LTcuMjg4aDE0LjMzMnYxNC41NzVINTMuNDQxek0zNC43MzcgODEuOTg0di03LjI4OGgxNS43ODl2MTQuNTc1SDM0LjczN3pNNzAuNjg4IDEwMC4wODF2LTcuODk1aDE1Ljc5djE1Ljc5aC0xNS43OXpNNTMuNDQxIDExOS4yNzF2LTcuMTY2aDE0LjMzMnYxNC4zMzJINTMuNDQxek0zNC43MzcgMTE5LjI3MXYtNy4xNjZoMTUuNzg5djE0LjMzMkgzNC43Mzd6TTcwLjY4OCAxMzguNzA0di03Ljg5NGgxNS43OXYxNS43ODloLTE1Ljc5ek03MC42ODggMTU4LjAxNnYtNy4yODdoMTUuNzl2MTQuNTc1aC0xNS43OXpNNTMuNDQxIDE1OC4wMTZ2LTcuMjg3aDE0LjMzMnYxNC41NzVINTMuNDQxeiIgc3R5bGU9ImZpbGw6IzU5YTdhNTtzdHJva2U6bm9uZTtzdHJva2Utd2lkdGg6LjI0MjkxNTtmaWxsLW9wYWNpdHk6MSIgdHJhbnNmb3JtPSJzY2FsZSguOCkiLz48L3N2Zz4=)
![Amazon S3](https://img.shields.io/badge/Amazon%20S3-333333?style=flat&logo=amazons3)

## 📬 Contato

<p align="justify">
  Se você tiver dúvidas ou sugestões, pode me encontrar em <a href="mailto:daniel.braz@vyox.io">daniel.braz@vyox.io</a> ou através do <a href="https://www.linkedin.com/in/dbrazl/">LinkedIn</a>.
</p>
