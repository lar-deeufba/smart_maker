# Impressora 3D Smart Maker

Instruções para impressão com a impressora 3D Smart Maker do LaR.


- [Introdução](#introduction)
- [Modelagem](#modelling)
- [Configurações Adicionais](#config)
- [Configurando Simplify3D No linux](#usage)
- [Vocabulário](#vocab)
- [Exemplo](#example)


### <a name="introduction"></a> Introdução
Caso você não seja habituado com alguns jargões de impressão 3D, veja a seção de [vocabulário](#vocab).
- Este manual prevê o uso de ABS. 
- Temperatura da extrusora: 230 graus
- Temperatura da mesa: 110 graus

Configurações prontas para os respectivos Slicers podem ser encontradas nas pastas ``` /Simplify3DConfig ``` ou ``` /CuraConfig ```. A vantagem do Cura se deve ao fato de ser gratuito.

No Simplify3D basta usar a opção de ``` Import profile ``` e escolher o arquivo de extensão ``` .fff ```, note que o arquivo de configuração não vem com as opções de Skirt, Raft ou Suporte e que estes devem ser configuradas pelo usuário. (MELHORAR ESSE TRECHO)

No nosso caso, sugiro que escolhemos ``` SmartMakerSemSuporte.fff ``` como o profile para as impressões.

<!-- Colocar link do pdf original com as instruções -->

### <a name="modelling"></a> Modelagem

Caso queira modelar alguma peça que envolva furo/corte/encaixe, uma dica extremamente importante é dar um offset em ambas as peças.

Na peça "macho" 0.6mm **maior**.

Na peça "fêmea" 0.6mm **menor**.

Onde 0.6mm é o tamanho do nozzle.

### <a name="config"></a> Configurações Adicionais

Adicionar Skirt para expelir o filamento não desejado no início da impressão

### <a name="usage"></a> Usando Simplify3D no Linux

Para instalar o Simplify3D (Slicer recomendado além do Cura) acesse [aqui](https://github.com/lar-deeufba/simplify3d_linux) e **siga as instruções do README** (disponível para membros do Time do LaR no GitHub).

Caso queira imprimir conectado ao computador é necessário liberar os direitos da porta:

``` $ sudo chmod 666 /dev/ttyUSB0 ```

ou

``` $ sudo chmod 666 /dev/ttyACM0 ```

Após isso é só escolher o baudrate ``` 115200 ``` e clicar em ``` connect ```.

<!-- Colocar imagem aqui -->



### 

### <a name="vocab"></a> Vocabulário
- Extrusora = componente que realiza o depósito do filamento (polímero)
- Nozzle = bico da extrusora
- Slicer = fatiador para gerar o arquivo ``` .gcode ```
- Skirt = saia
- Raft =

### <a name="example"></a> Exemplo
Na pasta ``` Example ``` há um arquivo  ``` .STL ```, que é um cilindro com diâmetro de 10mm e 5mm de altura. Iremos gerar o ``` .gcode ``` a partir dele utilizando o Simplify3D. Neste caso iremos realizar a impressão a partir do computador. Caso prefira, há a versão deste tutorial em forma de video, clique [aqui]() para vê-lo.

Caso queira imprimir utilizando o cartão de memória, basta lembrar que o mesmo deve estar formatado com o cluster ``` FAT32 ```.


<!-- Colocar imagens e fornecer arquivos exemplo -->
