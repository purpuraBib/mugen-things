<tt>[This file is copylefted]</tt>

Addresses make ESP+8 be return address
<div>
4CA is an address to adjust stack and return to the substituted DTC Text.

Instructions placed in 4CA(0x414334) are:
```
winmugen.exe+14334 - 83 C4 08              - add esp,08 { adjusts stack }
winmugen.exe+14337 - C3                    - ret  { returns to substituted DTC Text }
```
</div>

#### EBP = Clipboard addr., EBX = Addr. to substituted DTC Text
```
U-@   ,A, SXA, ,kA, P=B, [=B, u?B, [GB, I*E, z*E, 3-E, O-E, nCE, >2G, C3G, p3G, -7G, S7G, F9G, b:G, #<G, A<G, _<G, M?G, *@G,
P@G, 0BG, KCG, tCG, ,DG, dDG, NEG, wEG, yFG, XGG, lHG, ,IG, pJG, aNG, ZbG, }bG, ,cG, RcG, xcG, vfG, 7gG, 8pG, bpG, 'qG, EqG,
fqG, 8rG, \rG, LsG, 5wG, jwG, $(G, ?>H, 9KH, ixH, [#I, +ZI
```
#### EDI, ESI
```
#H@, ^H@, eH@, [^A, x`C, ]`G, 12H, '=H, K=H, _?H, -BH, BlH, =wH, ZwH, vwH, lzH, -3I
```
#### EDI, EBX
```
>gD, #7H
```
#### ESI, EBX
```
2-A, 61A, PrA, [GB, bIB, E$D, 4&E, `.E,  /E, j1E, j6E, *7E, O?E, 0uG, b<H, m<H, `@H, xJH, ~JH, .TH, d4I, K5I
```
#### ESI, EBP
```
nhH, C6I, >`I
```
#### ESI, ECX
```
1@A
```
#### ESI, EDI
```
w0I
```
#### EBX, ECX
```
J5B, 8`C, |HH, +vH
```
#### EAX, EBP
```
qxI, i+I (n+I, r+I jmps to i+I)
```
#### EBX, ECX, EAX = 0
```
2EA (4EA will save EAX)
```
#### EBX, ECX, EAX = -1
```
}:H
```
#### EBX, ESI, EAX = 0
```
kNH
```
#### EBX, ESI, EAX = 1?
```
pNH (rNH will make EAX -1)
```
#### ESI, EBX, EAX = 0
```
^6B, d@H
```
#### ESI, EBX, EAX = an any minus number?
```
MuG
```
#### EBP, EBX, EAX = 0
```
)rC, H/G, wBG, 9dG, |dG, weG, D>H, !NH
```
#### EBP, EBX, EAX = 1
```
2I@,  rC, |3G, <gG, pvG
```
#### EBP, EBX, EAX = -0x66
```
^gH, ogH
```
#### EBP, EBX, EAX = 0?
```
o7G, gxG (q7G, ixG will make EAX any minus number)
```
#### EBP, EBX, then \[EAX+ECX] = 0
```
BKH
```
#### EBP, EBX, EAX = EDX
```
ePD
```
#### ECX, ESI, EAX = -1?
```
S3I (U3I will make EAX 0)
```

#### ESI, EBX, [EDX] = 00000000
```
!^H
```
<hr>

#### May works but how to use
```
:4A
```
#### ESI = Addr. to substituted DTC Text
```
L3A, .}A, &&D, 8&D
```
#### ECX = Addr. to substituted DTC Text
```
3JI, zKI, 7bI
```
