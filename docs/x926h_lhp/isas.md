# X926-H Long Heap Support Instruction Set

Copyright Advanced Digitech Studio

## Content

1. Long memory write & read

## Long memory write & read

| Name | Opcode | Feature |
|:-- |:-- |:-- |
| lodl |  0x2C  | Use the top stack item as address to load 8 values, result will put to the stack. |
| strl |  0x2D  | Use the first top stack item as address and use the second top stack item as 8 8-bit values store to the memory. |