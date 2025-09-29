📄 Descrição do Projeto
Este repositório contém o código-fonte e os recursos do Trabalho de Conclusão de Curso (TCC) focado no desenvolvimento de um sistema de classificação de imagens de folhas utilizando técnicas de Machine Learning/Deep Learning.

O objetivo principal é treinar um modelo capaz de identificar ou classificar diferentes tipos de folhas (ou detectar doenças/condições) a partir de imagens de entrada. O projeto inclui o pipeline completo, desde o pré-processamento dos dados até a disponibilização de uma aplicação web simples para testes (via app.py).

🛠️ Tecnologias Utilizadas
O projeto é desenvolvido em Python e utiliza as seguintes principais tecnologias:

Linguagem de Programação: Python
Web Framework (Interface): Flask (ou similar, deduzido por app.py)
Machine Learning/Deep Learning: Bibliotecas como TensorFlow, PyTorch ou Scikit-learn (dependendo da implementação em train_model.py)
Manipulação de Dados: Pandas, NumPy (Geralmente utilizado em projetos ML)

📁 Estrutura do Repositório
Arquivo/Pasta	Descrição
data/	Pasta destinada a dados intermediários ou resultados do modelo.
dataset/	Contém o conjunto de dados de imagens de folhas utilizado para treinamento e teste do modelo.
app.py	Aplicação principal que expõe o modelo treinado, possivelmente uma API ou interface web simples.
train_model.py	Script para pré-processar os dados e treinar o modelo de classificação.
predict_leaf.py	Módulo que encapsula a lógica de carregamento do modelo e realização de previsões em novas imagens.
classes.json	Arquivo de configuração contendo a lista das classes (rótulos) que o modelo é capaz de prever.
.gitignore	Especifica arquivos e pastas que devem ser ignorados pelo Git (como ambientes virtuais e modelos grandes).

# 🚀 Como Executar o Projeto
Siga os passos abaixo para configurar e executar o projeto localmente.

Pré-requisitos
Python 3.x
Pip (gerenciador de pacotes)

# 1. Clonar o Repositório

Bash
git clone https://github.com/Pedrocasbar/tcc-.git
cd tcc-

# 2. Configurar o Ambiente
É altamente recomendado o uso de um ambiente virtual:

Bash
python -m venv venv
source venv/bin/activate  # Linux/macOS
venv\Scripts\activate   # Windows

# 3. Instalar Dependências
Crie um arquivo requirements.txt com as dependências do projeto e instale-as (assumindo que você as listará lá):

Bash
 Exemplo de conteúdo do requirements.txt:
 tensorflow
 flask
 opencv-python
 numpy
 pandas

Bash
pip install -r requirements.txt

# 4. Treinar o Modelo (Opcional)
Se você alterou o dataset ou deseja retreinar o modelo:

Bash
python train_model.py

# 5. Executar a Aplicação
Inicie o servidor local através do app.py:

Bash
python app.py
A aplicação estará disponível em http://127.0.0.1:5000/ (ou outra porta configurada).

🧑 Autor: Pedro Castro Barros
