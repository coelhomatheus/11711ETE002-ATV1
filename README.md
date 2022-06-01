# 11711ETE002-ATV1
## Matheus Rodrigues Cunha Coelho
### Repositório ATV1 - Sistemas Embarcados I

Inicialmente, instalamos e configuramos o ambiente, intalamos o *Ubuntu 20.04* no *Wsl*. Nele criamos os primeiros arquivos que seriam usados no STM32F411, também tivemos o primeiro contato com arquivos *Makefile*, que são responsáveis por automatizar a compilação dos scripts.

Após feitas toda a configuração e preparação do espaço onde trabalhariamos, foi feito o desenvolvimento dos códigos que seriam usados no chip, para verificar se o funcionamento estava correto tinhamos como objetivo final criar um projeto que tem a função de piscar um LED, contido na *BlackPill*. Para isso criamos os códigos contidos na pasta **Src**. Nos códigos, configuramos os vetores de interrupção, já que o ARM Cortex-M não póssui um sistema operacional, que fica responsabilizado por essa parte, também com o auxílio do *datasheet* do nosso chip, definimos os endereços de registradores e habilitamos a porta GPIOC, vale ressaltar no STM32F411 o LED está no pino 13. Também foi criado um arquivo *linker* que é responsável por unir os códigos e gerar o executável e controlar a memória.
