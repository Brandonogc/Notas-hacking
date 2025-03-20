**Reto:** binhexa

**Descripción:**
¿Qué tan bien puedes realizar operaciones binarias básicas?Empieza a buscar la bandera aquí`nc titan.picoctf.net 57864`

**Solución:**
brandonogc0107-picoctf@webshell:~$ nc titan.picoctf.net 57884

Welcome to the Binary Challenge!"
Your task is to perform the unique operations in the given order and find the final result in hexadecimal that yields the flag.

Binary Number 1: 10000001
Binary Number 2: 10111010


Question 1/6:
Operation 1: '|'
Perform the operation on Binary Number 1&2.
Enter the binary result: ^C
brandonogc0107-picoctf@webshell:~$ nc titan.picoctf.net 57884

Welcome to the Binary Challenge!"
Your task is to perform the unique operations in the given order and find the final result in hexadecimal that yields the flag.

Binary Number 1: 00000011
Binary Number 2: 01001110


Question 1/6:
Operation 1: '+'
Perform the operation on Binary Number 1&2.
Enter the binary result: 1010001
Correct!

Question 2/6:
Operation 2: '|'
Perform the operation on Binary Number 1&2.
Enter the binary result: 01001111
Correct!

Question 3/6:
Operation 3: '>>'
Perform a right shift of Binary Number 2 by 1 bits .
Enter the binary result: 100111
Correct!

Question 4/6:
Operation 4: '&'
Perform the operation on Binary Number 1&2.
Enter the binary result: 00000010
Correct!

Question 5/6:
Operation 5: '*'
Perform the operation on Binary Number 1&2.
Enter the binary result: 00000010
Incorrect. Try again
Enter the binary result: 10
Incorrect. Try again
Enter the binary result: 11101010
Correct!

Question 6/6:
Operation 6: '<<'
Perform a left shift of Binary Number 1 by 1 bits.
Enter the binary result: 110
Correct!

Enter the results of the last operation in hexadecimal: 6

Correct answer!
The flag is: picoCTF{b1tw^3se_0p3eR@tI0n_su33essFuL_aeaf4b09}

**Notas adicionales:**

**Referencias:** 
https://www.rapidtables.com/calc/math/binary-calculator.html
https://www.rapidtables.com/convert/number/binary-to-hex.html