# sprintf_Tutorial
 quick lookup guide for using the sprintf function
 


 



## [Specifier]
| Character | Data Type                                             | Example |
|---        |---                                                    |---      |
|d or i     |  Signed decimal integer                               | 392     |  
|u          |Unsigned decimal integer                               |  7235   |
|o          |Unsigned octal                                         |  610    |
|x          |Unsigned hexadecimal integer                           | 7fa     |
|X          |Unsigned hexadecimal integer (uppercase)               |  7FA    |
|f          |Decimal floating point, lowercase                      | 392.65  |
|F          |Decimal floating point, uppercase                      |392.65   |
|e          |Scientific notation (mantissa/exponent), lowercase     | 3.9265e+2|
|E          |Scientific notation (mantissa/exponent), uppercase     |3.9265E+2 |
|g          |Use the shortest representation: %e or %f              |392.65    |
|G          |Use the shortest representation: %E or %F              | 392.65   |
|a          |Hexadecimal floating point, lowercase                  |-0xc.90fep-2|
|A          |Hexadecimal floating point, uppercase                  |-0XC.90FEP-2|
|c          |Character                                              |a          |
|s          |String of characters                                   | sample    |
|p          |Pointer address                                        |b8000000   |
|n          |Nothing printed.                                       |          |
|lu         |Unsigned LONG                                          |          |

- The corresponding argument must be a pointer to a signed int. 
- The number of characters written so far is stored in the pointed location.  
- % A % followed by another % character will write a single % to the stream.  %


## [Flags]

|Character | Action       | Notes |
|---       |---           |---    |
|-         | Left-Justify |
| +        | Force sign   |(- or +)|
|" " (space)| No Sign     |
|#          |add leading zeros |(in specific cases). with floats forces decimal point|
|0          |Left Pad with Zeros||


## [Width]

|Character | Action | Notes |
|---       |---     |---    |
|(number)  | Number of characters printed. |Padded with spaces
|*         |width is not specified but passed as an additional integer| as an argument *eg: |

```
 int widthValue = 20;
 sprintf(screenBuffer[3], "%*c", widthValue, downArrow);
```

## [Precision] 

|Character | Action | Notes |
|---       |---     |---    |
|.(number) |  for integers number of digits, for floats number of digets after decimal | defaults to 1 |
|.*        |  precision not specified but passed as additional int value| |

## [Length]

|Character | Action   | Notes |
|---       |---       |---    |
|h         | short int|       |
|I         | long int or unsigned int|
|L         | Long Double (only floating points)|


# % [Flags] [Width] [.Precision] [Length] [Specifier] 

`% [Flags] [Width] [.Precision] [Length] [Specifier]`








### ASCII Help

| ASCII Value Range | Character Type | Notes |
|---                |---             |---    |
|32:                | " "      space |       |
| 33 - 47           | Punctuation    |       |
| 48 - 57           |  0 to 9        |       | 
|58 - 64            |  Punctuation   |       |
| 65 - 90           |  A - Z         |       | 
| 91 - 96           |  Punctuation   |       |
| 97 -              |                |       |

