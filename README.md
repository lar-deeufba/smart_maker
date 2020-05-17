# Impressora 3D Smart Maker

Instruções para impressão com a impressora 3D Smart Maker do LaR.

<p align="center">
  <a href="#introduction">Introdução</a> •
  <a href="#modelling">Modelagem</a> •
  <a href="#config">Configurações Adicionais</a> •
  <a href="#vocab">Vocabulário</a> •
</p> 

### <a name="introduction"></a> Introdução
Caso você não seja habituado com alguns jargões de impressão 3D, veja a seção de vocabulário <a name="introduction"></a>.
O manual prevê o uso de ABS. 
Temperatura da extrusora: 230 graus

Configurações prontas para os respectivos Slicers podem ser encontradas nas pastas ``` /Simplify3DConfig ``` ou ``` /CuraConfig ```. A vantagem do Cura é que este é multiplataforma e gratuíto.

No Simplify3D basta usar a opção de ``` Import profile ``` e escolher o arquivo de extensão ``` .fff ```, note que o arquivo de configuração não vem com as opções de Skirt, Raft ou Suporte e que estes devem ser configuradas pelo usuário. (MELHORAR ESSE TRECHO)


### <a name="modelling"></a> Modelagem

Caso queira modelar alguma peça que envolva furo/corte/encaixe, uma dica extremamente importante é dar um offset em ambas as peças.

Na peça "macho" 0.6mm MAIOR

Na peça "fêmea" 0.6mm menor

Onde 0.6mm é o tamanho do nozzle

### <a name="config"></a> Configurações Adicionais

Adicionar Skirt para expelir o filamento não desejado no início da impressão

### <a name="vocab"></a> Vocabulário
*Extrusora = componente que realiza o depósito do filamento (polímero)
*Nozzle = bico da extrusora
*Slicer = fatiador para gerar o arquivo ``` .gcode ```
*Skirt = saia
*Raft =