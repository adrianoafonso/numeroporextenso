# numeroporextenso

Número por Extenso, versão 2.0.3 (07/03/2013)
Desenvolvido por Noelson A. Duarte e Gustavo B. Pacheco

Plugin LiBo que permite escrever números por extenso.


Valor por extenso no LibreOffice
=================================

Histórico:
----------
1 sem 2006 -> Vitório Furusho sugere o desenvolvimento de uma função para gerar valores por extenso em várias moedas
12/07/2006 -> versão 1b1, liberada como suplemento - Noelson Duarte
08/04/2009 -> versão 1.0, liberada como extensão - Noelson Duarte 
06/04/2011 -> versão 2.0, suporte ao OOo e ao LibreOffice - Noelson Duarte
20/04/2011 -> versão 2.0.1, atualização para as regras da nova ortografia (retirada do trema) - Gustavo Pacheco
21/04/2011 -> versão 2.0.1, integração com menu Inserir - Gustavo Pacheco.
23/04/2011 -> versão 2.0.2, novos ícones, substituição das referências BrOffice.org para LibreOffice - Gustavo Pacheco.
07/03/2013 -> versão 2.0.3, troca de Mid$ por Split na função eliminaPontos - Gustavo Pacheco.


Melhorias:
Versão 2.0 
- Corrigido erro durante a instalação (node desconhecido)

O que faz a extensão ?
------------------------
Escreve valores numéricos (simples ou em R$) por extenso num documento do Writer ou numa célula de uma planilha. Para células, não se trata de uma função a ser usada como =funcao(a1). O suplemento escreve o extenso na célula ativa. Para aqueles que necessitam de uma função, consultem o item Funcao para o Calc.

Como instalar o suplemento ?
----------------------------
Para um usuário
1)Ferramentas | Gerenciador de Pacotes | selecione <Meus pacotes> | comande <Adicionar>
2)No diálogo de seleção de pacote, localize o arquivo BrOo_Extenso.zip e comande <Abrir>

Reinicie o LibreOffice, surge uma nova barra de ferramenta com um ícone [ nE ]. Em Ferramentas => Suplementos será acrescentada a opção <BrOffice> | <Número por extenso>.

Para todos os usuários da instalação do LibreOffice
----------------------------------------------------
Obs: para instalar, precisa dos direitos

1)<broo_install>/program/unopkg gui <Enter>
2)No diálogo, selecione Pacotes do LibreOffice, comande <Adicionar>
3)No diálogo de seleção de pacote, localize o arquivo BrOo_Extenso.zip e comande <Abrir>

Reinicie o LibreOffice, surge uma nova barra de ferramenta com um ícone [ nE ]. Em Inserir será acrescentada a opção <Número por extenso>.

Atenção: o suplemento, apesar de não testado, pode ser instalado nas versões do OOo 1.1.x.

Como usar o suplemento ?
------------------------
No Writer:
----------

Digite o valor e execute a macro

Selecione o valor e execute a macro

Posicione o cursor sobre o valor e execute a macro

Se o cursor não estiver sobre um valor numérico, uma caixa de diálogo será exibida, digite o valor e pressione o botão <Ok>.

Obs: ao obter o valor do documento, a ferramenta assume, por padrão, que o extenso refere-se a uma moeda ( acrescenta reais e centavos ). A caixa de diálogo permite outras variações.

No Calc:
--------

Selecione a célula de destino

Execute a macro, uma caixa de diálogo será exibida, digite o valor e pressione o botão <Ok>.

Atenção:
Existem alguns testes simples de validação do valor numérico. Mas o responsável pela digitação e formatação correta deste valor é o usuário.

Funcão para o Calc
------------------
Se você precisa de uma função, semelhante às funções do Calc (uso como fórmula numa célula), baixe o arquivo ValorExtenso.sxc e instale a função NExtenso.

Ajude-nos
---------

Temos como meta integrar estas ferramentas ao LibreOffice (o suplemento e a função para o Calc). Participe também, precisamos da sua ajuda para:

- Testar a ferramenta e informar defeitos;
- Sugerir melhorias; se não tiver nada em mente, consulte os tópicos a seguir.

Por fazer no suplemento
-----------------------
- Definir nomes adequados para as entradas de menu em < Ferramentas | Suplementos >.
- Escrever o extenso em objetos de desenho (texto, retângulo, etc).
- Verificar a correção gramatical do extenso. Alguns autores aceitam vírgula, outros não.
- É preciso formatar e substituir valor numérico ? (separadores, símbolo da moeda, etc)
- É necessário aumentar o limite do valor numérico (na ordem dos quatrilhões) ?
- Adicionar outras unidades (monetárias ou não) ao diálogo ?
- Data por extenso, alguém usa ?

Mal funcionamento no suplemento
-------------------------------

- Valores digitados como ,xx são interpretados como inteiro e não como fração.
- Não trabalha com texto dentro de objetos de desenho

Desenvolvedores
---------------
Noelson Alves Duarte e Gustavo Buzzatti Pacheco

Críticas e sugestões
--------------------
noelsonalvesATyahoo.com ou gbpachecoATgmail.com
