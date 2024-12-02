# InstantMesh: Geração Eficiente de Malhas 3D a Partir de uma Única Imagem

## Introdução
**InstantMesh** é uma ferramenta avançada desenvolvida pela TencentARC para a geração eficiente de malhas 3D a partir de uma única imagem. Utilizando uma combinação inovadora de técnicas de difusão multiview e reconstrução esparsa (LRM - Large Reconstruction Model), o InstantMesh consegue criar malhas tridimensionais detalhadas de forma rápida e precisa. Este modelo é especialmente útil em áreas como design de produtos, jogos, animações, medicina e educação.

## Principais Características
### Eficiência na Geração
- **Tempo Rápido:** Capaz de gerar uma malha 3D em aproximadamente 10 segundos.
- **Algoritmo de Difusão Multiview:** Gera múltiplas vistas do objeto a partir de uma única imagem, captando diferentes ângulos e detalhes.

### Alta Precisão
- **Supervisões Geométricas:** Utiliza mapas de profundidade e normais de superfície para melhorar a qualidade e a precisão das malhas.
- **Reconstrução Esparsa (LRM):** O modelo aplica técnicas de aprendizado profundo para criar uma malha inicial e refiná-la, resultando em um modelo tridimensional detalhado.

### Facilidade de Integração
- **Compatibilidade:** O InstantMesh é compatível com ferramentas populares de aprendizado de máquina e processamento de imagens como Python, PyTorch, OpenCV e NumPy.

## Como Usar

### Pré-requisitos
Para utilizar o InstantMesh, você precisará dos seguintes pré-requisitos:
- **Python 3.8 ou superior.**
- **PyTorch 1.8.1 ou superior.**
- **Bibliotecas adicionais: OpenCV, NumPy.**

### Passos para Instalação e Execução

1. **Clonar o Repositório**
   ```bash
   git clone https://github.com/TencentARC/InstantMesh
   
2. **Instalar as Dependências**
   ```bash
    pip install -r requirements.txt
   
3. **Baixar os Modelos**

- **Os modelos podem ser baixados automaticamente pelo script de inferência ou manualmente e colocados na pasta ckpts/.**

4. **Executar o Modelo**

- **Demo Local:** Iniciar o demo com:
   ```bash
    python app.py
   
- **Geração de Malhas via Linha de Comando:**
   ```bash
    python run.py configs/instant-mesh-large.yaml examples/hatsune_miku.png --save_video

   
### Execução com Docker
Caso prefira utilizar Docker, siga os passos abaixo:

1. **Construir a Imagem Docker**
   ```bash
    docker build -t instantmesh .

2. **Executar o Contêiner Docker**
   ```bash
    docker run -p 8080:8080 instantmesh
   
### Limitações
Apesar de suas capacidades avançadas, o InstantMesh possui algumas limitações:

- **Dependência da Qualidade da Imagem:** A precisão da malha 3D gerada depende fortemente da qualidade da imagem de entrada.
- **Requisitos Computacionais:** A execução eficiente do modelo pode exigir hardware robusto, especialmente GPUs.
- **Escopo Limitado:** O modelo é otimizado para certos tipos de objetos e cenários, podendo não fornecer resultados ideais para todas as aplicações.

### Política de Uso
## Licença:
InstantMesh é distribuído sob a licença Apache-2.0, permitindo uso, modificação e distribuição dentro dos termos especificados.

## Contribuições
Contribuições para o projeto são bem-vindas. Se você tiver sugestões ou melhorias, por favor, envie um pull request ou abra uma issue no GitHub.

### Uso Ético
## Os usuários devem respeitar normas éticas e legais ao utilizar o InstantMesh, especialmente no que diz respeito à privacidade e direitos autorais.

### Resultados

