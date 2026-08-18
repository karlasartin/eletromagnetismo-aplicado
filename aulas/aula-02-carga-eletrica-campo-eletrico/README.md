# Aula 02 — Carga Elétrica e Campo Elétrico

## Eletromagnetismo Aplicado

Nesta aula estudaremos os fundamentos da **carga elétrica** e do
**campo elétrico**, estabelecendo a relação entre carga, força elétrica
e a modificação do espaço ao redor de uma carga fonte.

---

## Objetivos da Aula

Ao final desta aula, o estudante deverá ser capaz de:

- compreender o conceito de carga elétrica;
- identificar cargas positivas e negativas;
- compreender conservação e quantização da carga;
- analisar atração e repulsão entre cargas;
- aplicar a Lei de Coulomb;
- compreender o conceito de campo elétrico;
- diferenciar força elétrica de campo elétrico;
- determinar o campo produzido por uma carga puntiforme;
- identificar direção e sentido do campo elétrico;
- interpretar linhas de campo elétrico;
- aplicar o princípio da superposição;
- calcular o campo elétrico resultante;
- relacionar os conceitos estudados com aplicações em Engenharia.

---

## 1. Carga Elétrica

A carga elétrica é uma propriedade física fundamental da matéria.

As cargas podem ser:

- positivas;
- negativas.

A unidade de carga elétrica no Sistema Internacional é o coulomb (C).

### Carga elementar

e = 1,602 × 10⁻¹⁹ C

### Quantização da carga

q = n · e

---

## 2. Interação entre Cargas

Cargas de mesmo sinal se repelem.

Cargas de sinais diferentes se atraem.

---

## 3. Lei de Coulomb

A força elétrica entre duas cargas puntiformes é determinada por:

F = k · |q₁q₂| / r²

onde:

- F = força elétrica (N);
- q₁ e q₂ = cargas elétricas (C);
- r = distância entre as cargas (m);
- k ≈ 8,99 × 10⁹ N·m²/C².

---

## 4. Do conceito de força para o conceito de campo

Uma carga elétrica modifica o espaço ao seu redor.

CARGA FONTE
      ↓
modifica o espaço
      ↓
CAMPO ELÉTRICO
      ↓
colocamos uma carga de prova
      ↓
FORÇA ELÉTRICA

A carga de prova permite investigar o campo, mas não é responsável
pela existência dele.

---

## 5. Campo Elétrico

O campo elétrico é definido pela relação:

E = F / q₀

onde:

- E = campo elétrico;
- F = força elétrica;
- q₀ = carga de prova.

Unidade:

N/C

---

## 6. Campo produzido por uma carga puntiforme

Combinando a definição de campo elétrico com a Lei de Coulomb:

E = k · |Q| / r²

O campo depende:

- da carga fonte Q;
- da distância r até o ponto analisado.

---

## 7. Direção e Sentido

### Carga positiva

O campo elétrico aponta para fora da carga.

### Carga negativa

O campo elétrico aponta em direção à carga.

---

## 8. Linhas de Campo Elétrico

As linhas de campo:

- saem das cargas positivas;
- chegam às cargas negativas;
- indicam a direção e o sentido do campo;
- apresentam maior densidade onde o campo é mais intenso;
- nunca se cruzam.

---

## 9. Princípio da Superposição

Quando várias cargas produzem campo em um mesmo ponto:

E⃗R = E⃗1 + E⃗2 + ... + E⃗n

Por componentes:

Ex = Σ Ei cos(θi)

Ey = Σ Ei sin(θi)

ER = √(Ex² + Ey²)

---

## 10. Hands On — Python

### Calculadora de Campo Elétrico

```python
k = 8.99e9

Q = float(input("Digite a carga Q em C: "))
r = float(input("Digite a distância em metros: "))

E = k * abs(Q) / r**2

print("Campo elétrico =", E, "N/C")

if Q > 0:
    print("Sentido: para longe da carga.")
else:
    print("Sentido: em direção à carga.")
