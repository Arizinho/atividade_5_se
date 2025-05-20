# Simulação de Estação de Alerta de Enchentes

Este projeto foi desenvolvido utilizando a placa BitDogLab. Tem como objetivo simular uma estação de monitoramento de enchentes, utilizando sensores simulados por joystick, com sinalização visual e sonora em situações de risco.

O sistema funciona em dois modos:
- **Modo Normal:** exibe os valores simulados de nível da água e volume de chuvas no display OLED. Os demais periféricos permanecem desligados.
- **Modo Alerta:** ativado automaticamente quando o nível da água atinge 70% ou o volume de chuva 80%. Neste modo, o sistema acende o LED vermelho, ativa o buzzer, exibe uma mensagem de alerta no display OLED e mostra um símbolo de exclamação (!) na matriz de LEDs.

Todas as funcionalidades são implementadas como tarefas no FreeRTOS, que se comunicam por meio de filas.
