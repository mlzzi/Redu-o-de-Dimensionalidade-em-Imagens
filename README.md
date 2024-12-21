# 🌟 Conversão de Imagens com OpenCV e URLs 📸

Este código realiza a **conversão de imagens em tons de cinza ou preto e branco** diretamente a partir de uma URL. Ele utiliza as bibliotecas **OpenCV**, **Matplotlib** e **Requests** para manipular e visualizar imagens de forma prática e intuitiva. 🎨✨

---

## 🚀 Funcionalidades
- 🎯 **Ler imagens diretamente de uma URL.**
- 🖤 **Converter imagens para tons de cinza.**
- ⚫ **Converter imagens para preto e branco com ajuste de limiar.**
- 🖼️ **Visualizar imagens originais e processadas lado a lado.**

---

## 📚 Bibliotecas Utilizadas
1. **OpenCV (`cv2`)**: Manipulação e processamento de imagens. 🖌️
2. **NumPy (`np`)**: Suporte para arrays e operações matemáticas. 🧮
3. **Matplotlib (`plt`)**: Exibição de gráficos e imagens. 📊
4. **Requests e PIL**: Leitura de imagens diretamente de URLs. 🌐

---

## 🏗️ Estrutura do Código

### 1. 🔗 Função para Ler Imagem de uma URL
Primeiro, a imagem é carregada da URL utilizando o **OpenCV** e a função `cv2.imread()`.

### 2. 🔗 Função para Conversão em Tons de Cinza
Esta função converte a imagem carregada para tons de cinza utilizando o `cv2.cvtColor()`, que transforma a imagem colorida em uma imagem em escala de cinza.

### 3. 🔗 Função para Conversão em Tons de Preto e Branco
Aqui, a imagem é convertida para **preto e branco** aplicando a técnica de limiarização (`cv2.threshold()`), onde valores acima de um certo limiar são convertidos para branco e os valores abaixo para preto. A suavização é aplicada antes da limiarização para melhorar o resultado.

### 4. 🔗 Função para Visualizar as Imagens
Usando o **Matplotlib**, as funções exibem a imagem original e a convertida lado a lado para facilitar a comparação.

---

## 💡 Como Usar

1. **Defina a URL da imagem que deseja processar:**
   ```python
   url_imagem = "https://www.midiorama.com/wp-content/uploads/2019/04/lena-meyer-landrut.png"
   ```
2. **Para converter a imagem para tons de cinza:**
   ```python
   converter_para_cinza(url_imagem)
   ```
3. **Para converter a imagem para preto e branco (com limiar ajustável):**
   ```python
   converter_para_preto_branco(url_imagem, limiar=160)
   ```
## Basta substituir o link da imagem em url_imagem e chamar uma das funções para obter a conversão desejada. As funções exibirão a imagem original e a imagem processada lado a lado. ✨
