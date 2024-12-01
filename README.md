# Intro-to-CS

 This repository is to collect codes for GroupProject 11 in UFUG1601 Intro to CS

## 项目简介
本项目旨在模拟红队与蓝队之间的辩论场景，并利用多种语言模型（包括 OpenAI 的 GPT-3.5-turbo、NVIDIA 的 Llama 模型）来生成辩论内容，同时通过 SparkAI 模型作为法官来评判双方论点的说服力，最终确定辩论的胜负结果。在程序开始时，您需要先输入一个轮数N，这样我们将会进行N轮的辩论，并且将双方的言论记录于debate_output.txt中。

## 安装步骤：
1、您需要将我们的Project 11文件夹克隆至本地（或直接下载）

2、您需要配置您的环境，以便运行我们的代码：

    pip install openai

    pip install sparkai

3、配置好环境以后，请运行Project 11 agent arena2.0，这是我们最新的版本。

## 使用方法
在出现：“请输入对话轮数：”后，输入想要的对话轮数，然后等待程序运行完毕。对话过程可以在debate_output.txt中查看，也可以在终端查看。

## 代码架构
Project 11

├── Main Script

│   ├── run_debate()

│   └── __main__

├── Imports

│   ├── time

│   ├── os

│   ├── requests

│   ├── openai

│   ├── ChatSparkLLM

│   ├── ChunkPrintHandler

│   └── ChatMessage

├── SparkAI API Configuration

│   ├── SPARKAI_APP_ID

│   ├── SPARKAI_API_SECRET

│   ├── SPARKAI_API_KEY

│   ├── SPARKAI_URL

│   ├── SPARKAI_DOMAIN

│   └── spark (ChatSparkLLM instance)

└── OpenAI API Configuration

    └── get_openai_client(api_key, base_url)

