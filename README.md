# tutorial-python
Introdução a Ciência da Computação - Felipe Viel

O arquivo chamado **'Exemplo_Morfologia.ipynb'** carrega um código cuja finalidade geral é processar imagens utilizando as bibliotecas OpenCV e NumPy. Logo, a função principal é fazer operações morfológicas em imagens em escala gray. Algumas operações envolvidas são: erosão, gradiente, dilatação, abertura, fechamento. Basicamente as operações morfológicas são alguns procedimentos computacionais de processamento de imagem que alteram estrutura dos objetos existentes em uma imagem (png, jpg, jpeg etc), utilizando as em si as operações.

(Explicação dos scripts em trechos em 'Exemplo_Morfologia.ipynb')
**Explicação do código em etapas:**
- O código possui a importação das bibliotecas: 'cv2' e 'numpy'. Para rodar no Google Colab é incluso também a 'cv2_imshow'.

- 'j.png', 'j_ruido.png' e 'j_furos.png' são carregados no ambiente. Em escala cinza por meio da função cv2.imread e atribuindo variáveis.

- Logo, é criada uma matriz chamada 'kernel' com dimensões 5x5, preenchida com o valor 1.

- Em seguida o script faz realiza a erosão e a dilatação na imagem "j.png" utilizando o kernel, duas vezes. Onde são armazenados nas variáveis 'erosion' e 'dilation'.

- É aplicada a operação de gradiente na imagem "j.png" utilizando o kernel.

- O código faz a abertura na imagem 'j_ruido.png' creio que seja para remoção de algumas 'sujeiras' presentes na imagem (Observação da imagem final, na base da dedução). Armazena em 'opening'

- Em seguida o fechamento na imagem 'j_furos.png'. Os resultados são armazenados em 'closing'.

- No final há a exibição visual das imagens resultantes das operações morfológicas.

Resultado no Google Colab
