# X926-H Heap Support Instruction Set

Copyright Advanced Digitech Studio

## Content

1. Basic memory write & read

## Basic memory write & read

| Name | Opcode | Feature |
|:-- |:-- |:-- |
| lodb |  0x15  | Use the top stack item as address to load a value, result will put to the stack. |
| lods |  0x16  | Use the top stack item as address to load 2 values, result will put to the stack. |
| lodi |  0x17  | Use the top stack item as address to load 4 values, result will put to the stack. |
| strb |  0x18  | Use the first top stack item as address and use the second top stack item store to the memory. |
| strs |  0x19  | Use the first top stack item as address and use the second top stack item as 2 8-bit values store to the memory. |
| stri |  0x1A  | Use the first top stack item as address and use the second top stack item as 4 8-bit values store to the memory. |