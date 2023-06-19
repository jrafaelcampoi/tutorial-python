# tutorial-python
Introdução a Ciência da Computação - Felipe Viel

O arquivo chamado **'Exemplo_Morfologia.ipynb'** carrega um código cuja finalidade geral é processar imagens utilizando as bibliotecas OpenCV e NumPy. Logo, a função principal é fazer operações morfológicas em imagens em escala gray. Algumas operações envolvidas são: erosão, gradiente, dilatação, abertura, fechamento. Basicamente as operações morfológicas são alguns procedimentos computacionais de processamento de imagem que alteram estrutura dos objetos existentes em uma imagem (png, jpg, jpeg etc), utilizando as em si as operações.

**Explicação do código:**
O código inicia importando as bibliotecas necessárias para a aplicação de operações morfológicas em imagens, como a biblioteca cv2 da OpenCV e a biblioteca NumPy. Além disso, é importado o módulo "cv2_imshow" para exibir as imagens no ambiente do Google Colab.

Em seguida, são carregadas três imagens a serem processadas: "j.png", "j_ruido.png" e "j_furos.png". Essas imagens são carregadas em escala de cinza usando a função cv2.imread e atribuindo variáveis.

É criada uma matriz chamada "kernel" com dimensões 5x5, preenchida com o valor 1. Essa matriz é utilizada como elemento estruturante para as operações morfológicas.

O código realiza as operações de erosão e dilatação na imagem "j.png" utilizando o kernel definido. Essas operações são realizadas duas vezes, indicadas pelo parâmetro "iterations = 2". Os resultados das erosões e dilatações são armazenados nas variáveis "erosion" e "dilation", respectivamente.

Em seguida, é aplicada a operação de gradiente morfológico na imagem "j.png" utilizando o kernel. Essa operação destaca as bordas dos objetos na imagem e o resultado é armazenado na variável "gradient".

O código aplica a operação de abertura morfológica na imagem "j_ruido.png" para remover ruídos e objetos pequenos. A operação de fechamento morfológico é aplicada na imagem "j_furos.png" para preencher lacunas e conectar componentes quebrados. Os resultados são armazenados nas variáveis "opening" e "closing", respectivamente.

Por fim, o código exibe as imagens originais e as resultantes das operações morfológicas, permitindo a comparação visual dos efeitos.
