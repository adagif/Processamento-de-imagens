## Quantização de Imagem em Tons de Cinza

Este código demonstra a quantização de uma imagem em tons de cinza usando Python com as bibliotecas `cv2` (OpenCV) e `matplotlib`. 

**Objetivo:**

O código realiza a quantização uniforme de uma imagem em tons de cinza para reduzir o número de níveis de cinza que a imagem pode conter. Isso é útil para:

- **Compressão de dados:** Reduzir a quantidade de informação necessária para armazenar a imagem.
- **Visualização:** Simplificar a imagem para fins de análise ou apresentação.

**Como funciona:**

1. **Carregamento da imagem:**
   - O código carrega uma imagem em tons de cinza usando `cv2.imread('images.jpeg', cv2.IMREAD_GRAYSCALE)`.
   - Verifica se a imagem foi carregada corretamente.

2. **Quantização da imagem:**
   - Define uma função `quantizar_imagem` que realiza a quantização uniforme.
   - A função calcula o intervalo entre o valor mínimo e máximo da imagem.
   - Divide o intervalo em `niveis_de_cinza` partes iguais.
   - Percorre cada pixel da imagem, arredondando seu valor para o nível de cinza mais próximo.
   - Cria uma nova imagem com os níveis de cinza quantizados.

3. **Exibição dos resultados:**
   - Usa o `matplotlib.pyplot` para plotar as imagens.
   - Plota a imagem original na primeira posição.
   - Plota as imagens quantizadas em posições diferentes na mesma figura, usando uma grade de 2 linhas e 4 colunas.
   - Mostra a figura com todas as imagens.

**Requisitos:**

- Python 3
- OpenCV (cv2)
- Matplotlib

**Como usar:**

1. **Instale as bibliotecas:**
   ```bash
   pip install opencv-python matplotlib
   ```
2. **Salve o código como um arquivo Python (por exemplo, `quantizacao.py`).**
3. **Renomeie `'images.jpeg'` para o nome do seu arquivo de imagem.**
4. **Execute o código:**
   ```bash
   python quantizacao.py
   ```
5. **Visualize os resultados:**  Uma janela com as imagens original e quantizadas será exibida.


