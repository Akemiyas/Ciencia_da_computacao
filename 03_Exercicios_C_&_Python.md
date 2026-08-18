## EXERCÍCIOS ALGORITMOS CAP. 3 (EM DIAGRAMA, PY. E C)

### CÁLCULO DA ÁREA DE UM CÍRCULO
**C:**
```c
#include <stdio.h>
int main() {
    float pi = 3.14159265;
    float raio, A;
    printf("Digite o raio da circunferencia\n");
    scanf("%f", &raio);
    A = pi * (raio * raio);
    printf("A area da circunferencia e %.2f\n", A);
    return 0;
}
```
**Python:**
```python
pi = 3.14159265
raio = float(input("Digite o raio da circunferencia\n"))
A = pi * (raio * raio)
print(f"A area da circunferencia e {A:.2f}")
```

### CÁLCULO DO SALÁRIO DE UM PROFESSOR
**C:**
```c
#include <stdio.h>
int main() {
    double HA, HT, PD, descontos, SB, SL;
    printf("Insira os valores: hora-aula, horas trabalhadas e percentual de desconto\n");
    scanf("%lf %lf %lf", &HA, &HT, &PD);
    SB = HA * HT;
    descontos = PD * SB;
    SL = SB - descontos;
    printf("Salario bruto: %.2lf\n Salario liquido: %.2lf", SB, SL);
    return 0;
}
```
**Python:**
```python
HA = float(input("Digite o valor da sua hora-aula\n"))
HT = float(input("Digite sua hora trabalhada mensal\n"))
PD = float(input("Digite o percentual de desconto em decimal\n"))
SB = HA * HT
Descontos = SB * PD
SL = SB - Descontos
print(f"Salario Bruto {SB}\nSalario Liquido {SL}\n")
```
