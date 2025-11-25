# FACTORIAL-OF-A-NUMBER
# FACTORIAL OF A NUMBER USING 8051 (Keil)

## AIM
To write and execute an Assembly language program to perform the factorial of a number using 8051 Keil.

---

## APPARATUS REQUIRED
- Personal computer with Keil software

---

## ALGORITHM
1. **Start**
2. **Input**: Read the number `n`.
3. **Initialize**:
   - Set factorial to `1`.
   - Set `i` to `1`.
4. **Loop**: While `i` is less than or equal to `n`:
   - Multiply factorial by `i`.
   - Increment `i` by `1`.
5. **Output**: Store or print the value of factorial.
6. **End**

---

## FLOWCHART
<img width="506" height="525" alt="image" src="https://github.com/user-attachments/assets/f3b47187-6f0f-490c-8704-f2973cb2b276" />


---

## PROGRAM
```asm
ORG 0000H
MOV DPTR,#4500H
MOVX A,@DPTR
MOV R0,A
INC DPTR
ACALL FACTORIAL
MOVX @DPTR,A
SJMP THIN
FACTORIAL:DEC R0
CJNE R0,#01H,PRODUCT
SJMP THICK
PRODUCT:MOV B,R0
MUL AB
ACALL FACTORIAL
THICK: RET
THIN:RET
END

```
OUTPUT



<img width="600" height="900" alt="MPMC(FACT)" src="https://github.com/user-attachments/assets/9a237fd5-4f22-4a46-bec5-c98b9378df6e" />










<img width="600" height="900" alt="MPMC(FACT1)" src="https://github.com/user-attachments/assets/2689d7bf-d1a6-42ba-a9e7-943548987212" />

---
MANUAL CALCULATIONS
![WhatsApp Image 2025-11-09 at 14 54 29_03d45be4](https://github.com/user-attachments/assets/4b919a79-31d7-421e-878b-b0f703f6c400)

---

RESULT

Thus, the factorial of a number was calculated and executed successfully using 8051 Keil.

---


