# Analisador de Fluxos

O projeto em questão será um Analisador de Fluxos, seja de pessoas ou objetos, baseado em sensores de infravermelho.
Equipe:
* Carlos Victor Gonçalves Moura - 515016
* Luis Carlos Rodrigues dos Anjos - 509022
* João Guilherme Alves Noronha de Morais - 511930
* Antonio Ermeson Pereira Alves - 511473
<hr>
A pasta PF-Micros desse repositório corresponde ao *STM32 Project*, com os arquivos necessários para abri-lo na IDE. As tecnolgias apresentadas em sala de aula utilizadas foram, resumidamente, a UART - Universal Asynchronous Receiver/Transmitter e um Timeer da GreenPill. O circuito de detecção de passagem de um objeto qualquer funciona com base em dois fototransistores em conjunto com dois leds emissores de infravermelho.<br><br>
Esses circuitos permitem enviar sinais para a GreenPill via GPIO - General Purpose Input/Output que são armazenados para envio posterior ao computador.<br><br>
Inicialmente foi pensado envio das informações a cada intervalo de tempo pre-determinado, para isso o uso de Timer e da função HAL_TIM_PeriodElapseCallback() ([clique aqui](https://hackmd.io/@0xff07/Sy8U-l7Ec)). Com isso, é possível usar um módulo conversor USB-TTL e estabelecer comunicação entre a GreenPill e o computador enviando dados periodicamentes. Estes dados podem ser visualizados via programa de terminal que trabalha com as portas COM (porta de comunicação do computador). Escolhemos o TeraTerm, que pode ser baixado pelo link: https://tera-term.softonic.com.br.<br<br>
O TeraTerm também disponibiliza um sistema de log automatizado que poderá ser melhor trabalhado no futuro ou em outros projetos.

![](https://github.com/ermeson-alves/Analisador-de-fluxos/blob/main/PF%20-%20Micros%20(1).png)


![](https://github.com/ermeson-alves/Analisador-de-fluxos/blob/main/Diagrama%20em%20branco%20(3).png)
