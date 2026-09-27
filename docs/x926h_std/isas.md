# X926-H Standard Instruction Set

Copyright Advanced Digitech Studio

## Content

1. Basic single byte without immediate instructions

2. Teleport with immediate value instructions

3. Stack operation instructions

4. Basic calculate instructions

5. Basic control instructions

## Basic single byte without immediate instructions

| Name | Opcode | Feature |
|:-- |:-- |:-- |
| none |  0x00  | No thing to do. |

## Teleport with immediate value instructions

| Name | Opcode |                 Feature                  | Bytes |
|:-- |:-- |:-- |:-- |
| putb |  0x01  | Put a 8-bit immediate integer to stack.  |   2   |
| puts |  0x02  | Put a 16-bit immediate integer to stack. |   3   |
| puti |  0x03  | Put a 32-bit immediate integer to stack. |   5   |

## Stack operation instructions

| Name | Opcode |                    Feature                    |
|:-- |:-- |:-- |
| rmvi |  0x04  | Remove a top stack item.                      |
| cpyi |  0x05  | Copy a top stack item to the top.             |

## Basic calculate instructions

| Name | Opcode | Feature |
|:-- |:-- |:-- |
| addi |  0x06  | Add the first stack item and the second stack item, result at the stack top. |
| subi |  0x07  | Subtract the first stack item and the second stack item, result at the stack top. |
| muli |  0x08  | Multiply the first stack item and the second stack item, result at the stack top. |
| divi |  0x09  | Divide the first stack item and the second stack item, result at the stack top. |
| modi | 0x0A | Mod the first stack item and the second stack item, result at the stack top. |
| negi | 0x0B | Negate the top stack item, result at the stack top. |

| Name | Opcode | Feature |
|:-- |:-- |:-- |
| andi |  0x0C  | Calculate and the first stack item and the second stack item, result at the stack top. |
| orsi |  0x0D  | Calculate or the first stack item and the second stack item, result at the stack top. |
| xori |  0x0E  | Calculate xor the first stack item and the second stack item, result at the stack top. |

| Name | Opcode | Feature |
|:-- |:-- |:-- |
| dvui |  0x0F  | Calulate unsigned divide the first stack item and the second stack item, result at the stack top. |
| mdui | 0x10 | Calulate unsigned mod the first stack item and the second stack item, result at the stack top. |

| Name | Opcode | Feature |
|:-- |:-- |:-- |
| llsi |  0x11  | Left shift the first stack item and the second stack item logically. |
| lrsi |  0x12  | Right shift the first stack item and the second stack item logically. |
| arsi |  0x13  | Arithmetic right shift the first stack item and the second stack item. |

## Basic control instructions

| Name | Opcode | Feature |
|:-- |:-- |:-- |
| jmp |  0x14  | If the first stack item is zero, absolute jump to the address on the second stack item. Otherwise, remove the first stack item and keep the second stack item. |