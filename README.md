
# Procesador Monociclo MIPS – Logisim Evolution

Este proyecto implementa un procesador **monociclo** en Logisim Evolution, capaz de ejecutar instrucciones MIPS tipo **R**

## ⚙️ Instrucciones implementadas

1. `addi $t3, $zero, 8`  
   → Carga el valor 8 en el registro `$t3`.

2. `srl $t4, $t3, 1`  
   → Desplaza lógicamente a la derecha el valor de `$t3` en 1 bit y guarda el resultado en `$t4`.

   ## 🧩 Componentes principales

- Program Counter (PC)
- ROM (Memoria de instrucciones)
- Unidad de Control
- Banco de registros
- ALU
- Extensor de bits
- Multiplexores
- Unidad de desplazamiento (`shifter`) para `SRL`

## ✅ Funcionalidad

- Cada instrucción se ejecuta en un solo ciclo de reloj.
- El procesador interpreta correctamente el campo `shamt` para operaciones de desplazamiento como `srl`.
- El resultado se puede observar directamente en los registros.
