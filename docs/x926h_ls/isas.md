# X926-H Long Support Instruction Set

Copyright Advanced Digitech Studio

## Content

1. Teleport with immediate value instructions

2. Stack operation instructions

3. Calculate with long instructions

## Teleport with immediate value instructions

| Name | Opcode | Feature | Bytes |
|:--|:--|:--|:--|
| putl | 0x1B | Put a 64-bit immediate integer to stack. | 9 |

## Stack operation instructions

| Name | Opcode | Feature |
|:--|:--|:--|
| rmvl | 0x1C | Remove the top long value (2 stack items). |
| cpyl | 0x1D | Copy the top long value (2 stack items) to the top. |

## Calculate with long instructions

| Name | Opcode | Feature |
|:--|:--|:--|
| addl | 0x1E | Add the first long value and the second long value, result at the stack top. |
| subl | 0x1F | Subtract the first long value and the second long value, result at the stack top. |
| mull | 0x20 | Multiply the first long value and the second long value, result at the stack top. |
| divl | 0x21 | Divide the first long value and the second long value, result at the stack top. |
| modl | 0x22 | Mod the first long value and the second long value, result at the stack top. |
| negl | 0x23 | Negate the first stack item and the second item, result at the stack top. |

| Name | Opcode | Feature |
|:--|:--|:--|
| andl | 0x24 | Calculate and the first long value and the second long value, result at the stack top. |
| orsl | 0x25 | Calculate or the first long value and the second long value, result at the stack top. |
| xorl | 0x26 | Calculate xor the first long value and the second long value, result at the stack top. |

| Name | Opcode | Feature |
|:--|:--|:--|
| dvul | 0x27 | Calculate unsigned divide the first long value and the second long value, result at the stack top. |
| mdul | 0x28 | Calculate unsigned mod the first long value and the second long value, result at the stack top. |

| Name | Opcode | Feature |
|:--|:--|:--|
| llsl | 0x29 | Left shift the first long value by the second stack item (1 item) logically. |
| lrsl | 0x2A | Right shift the first long value by the second stack item (1 item) logically. |
| arsl | 0x2B | Arithmetic right shift the first long value by the second stack item (1 item). |