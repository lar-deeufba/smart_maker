# Impressora 3D Smart Maker

Instruções para impressão com a impressora 3D Smart Maker do LaR.

- [Introdução](#introduction)
- [Instalação do Simplify3D No linux](#usage)
- [Exemplo: Imprimindo uma peça](#example)
- [Vocabulário](#vocab)
- [Modelagem](#modelling)
- [Configurações Adicionais](#config)

### <a name="introduction"></a> Introdução
Caso você não seja habituado com alguns jargões de impressão 3D, veja a seção de [vocabulário](#vocab). Como no laboratório têmos apenas filamento ABS, então **iremos pressupor SEMPRE o uso do ABS no manual**. No entanto, os arquivos de configuração para PLA fonecidos pelo fabricante podem ser encontrados neste repositório.

- Este manual prevê o uso de ABS.
- Temperatura da extrusora: 230 graus
- Temperatura da mesa: 110 graus

Configurações prontas para os respectivos Slicers podem ser encontradas nas pastas ``` /Simplify3DConfig ``` e ``` /CuraConfig ```. A vantagem do Cura se deve ao fato de ser gratuito. Neste README focaremos com o uso do Simplify3D, no entanto os arquivos de configuração fornecidos pelo fabricante para usar o Cura se encontram neste repositório.

### <a name="usage"></a> Instalação do Simplify3D no Linux

Para instalar o Simplify3D (Slicer recomendado além do Cura) acesse [aqui](https://github.com/lar-deeufba/simplify3d_linux) e **siga as instruções do README** (disponível para membros do Time do LaR no GitHub).

### <a name="example"></a> Exemplo: Imprimindo uma peça
Na pasta ``` Example ``` há um arquivo  ``` cilindro.STL ```, que é um cilindro com diâmetro de 10mm e 5mm de altura. Iremos gerar o ``` .gcode ``` a partir dele utilizando o Simplify3D. Neste caso iremos realizar a impressão a partir do computador. Caso prefira, há a versão deste tutorial em forma de video, clique [aqui]() para vê-lo.



Caso queira imprimir utilizando o cartão de memória, basta lembrar que o mesmo deve estar formatado com o cluster ``` FAT32 ```.

Caso queira imprimir conectado ao computador é necessário liberar os direitos da porta:

``` $ sudo chmod 666 /dev/ttyUSB0 ```

ou

``` $ sudo chmod 666 /dev/ttyACM0 ```

Após isso, basta escolher o baudrate ``` 115200 ``` e clicar em ``` connect ```.

Um exemplo de como deve ficar o painel:

![panel](https://user-images.githubusercontent.com/24254286/82366174-2dea1780-99e8-11ea-9775-775f433d3428.png)


### <a name="vocab"></a> Vocabulário
- ABS = filamento
- PLA = filamento
- Extrusora = componente que realiza o depósito do filamento (polímero)
- Nozzle = bico da extrusora
- Slicer = fatiador para gerar o arquivo ``` .gcode ```
- Skirt = saia
- Raft =

### <a name="modelling"></a> Modelagem

Caso queira modelar alguma peça que envolva furo/corte/encaixe, uma dica extremamente importante é dar um offset em ambas as peças.

Na peça "macho" 0.6mm **maior**.

Na peça "fêmea" 0.6mm **menor**.

Onde 0.6mm é o tamanho do nozzle.

### <a name="config"></a> Configurações Adicionais

Adicionar Skirt para expelir o filamento não desejado no início da impressão