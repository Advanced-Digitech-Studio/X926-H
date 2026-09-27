# X926-H Instruction Set General Norms

Copyright Advanced Digitech Studio

## Content

1. Needed devices

2. Stack location

3. Stack action

4. Inintialize norm

5. About bits norm

## Needed devices

|      Name      | Quantity |  Bits  |      Size      | Feature | Location |
|:-- |:-- |:-- |:-- |:-- |:-- |
|     Memory     |    1     | 8-bit  | Usually 1048576 | For heap. | Outermost layer. |
|      Stack      |    1     | 32-bit | Usually 65537  | For operation.        | Usually at memory address 0x00000008 ~ 0x004000C. |
| Stack Pointer   |    1     | 32-bit |        1        | Point to a stack item. | Usually at memory address 0x00000004 ~ 0x00000007. |
| Program Counter |    1     | 32-bit |        1        | Point to a opcode. | Usually at memory address 0x00000000 ~ 0x00000003 |

## Stack location

Usually 0x00000000 ~ 0x00000003 is the **program counter**, 0x00000004 ~ 0x0000007 is the **stack pointer**, 0x00000008 ~ 0x0004000C is the **stack items**. And the **stack grows downward**.

## Initialize norm

Usually stack is **initialize at memory 0x00000004**, 65537 items  (1 × Stack pointer, 65536 × Stack items). And code is **initialize at memory 0x0004000D**. If has data section, load to **behind the code end**. More section will at **behind every section**.

## About bits norm

Usually a slot is **32-bit** but **must be Big-edian based**.