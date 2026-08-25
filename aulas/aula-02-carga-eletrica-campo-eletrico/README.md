# Aula 02 — Carga Elétrica e Lei de Coulomb

## Eletromagnetismo Aplicado

Nesta aula estudamos os fundamentos da **carga elétrica** e das **interações eletrostáticas**, chegando à formulação e aplicação da **Lei de Coulomb**.

Além da abordagem física e matemática, utilizamos **Python no Google Colab** para desenvolver calculadoras aplicadas à Lei de Coulomb.

---

## Objetivos da aula

Ao final da aula, o estudante deverá ser capaz de:

- compreender o conceito de carga elétrica;
- identificar cargas positivas e negativas;
- compreender as propriedades fundamentais da carga elétrica;
- analisar atração e repulsão entre cargas;
- aplicar a Lei de Coulomb;
- interpretar a influência da distância sobre a força elétrica;
- relacionar força elétrica com as Leis de Newton;
- realizar conversões de unidades;
- relacionar corrente elétrica e quantidade de carga;
- desenvolver cálculos da Lei de Coulomb utilizando Python.

---

# 1. Carga elétrica

A **carga elétrica** é uma propriedade fundamental da matéria responsável pelas interações elétricas.

Existem dois tipos de carga:

- positiva (+);
- negativa (-).

A unidade de carga elétrica no Sistema Internacional é o:

**Coulomb (C)**

A carga elementar possui módulo:

e = 1,602 × 10⁻¹⁹ C

---

# 2. Quantização da carga

A carga elétrica é quantizada.

Isso significa que a quantidade de carga de um corpo ocorre em múltiplos inteiros da carga elementar:

Q = n · e

Onde:

- Q = carga elétrica total;
- n = número inteiro;
- e = carga elementar.

---

# 3. Propriedades da carga elétrica

Entre as principais propriedades estudadas estão:

### Interação

Cargas elétricas exercem forças umas sobre as outras.

### Conservação

Em um sistema isolado, a carga elétrica total permanece constante.

### Quantização

A carga elétrica ocorre em múltiplos inteiros da carga elementar.

### Aditividade

A carga total de um sistema corresponde à soma algébrica das cargas individuais:

Qtotal = q₁ + q₂ + ... + qₙ

### Invariância

A carga elétrica de uma partícula não depende do referencial inercial utilizado.

### Transferência

Cargas elétricas podem ser transferidas entre corpos por diferentes processos, como:

- atrito;
- contato;
- indução.

---

# 4. Interação entre cargas elétricas

A regra fundamental é:

### Cargas de mesmo sinal

**Se repelem.**

(+)(+) → repulsão

(-)(-) → repulsão

### Cargas de sinais opostos

**Se atraem.**

(+)(-) → atração

Portanto:

> Mesmo sinal → REPULSÃO  
> Sinais opostos → ATRAÇÃO

---

# 5. Lei de Coulomb

A Lei de Coulomb determina o módulo da força eletrostática entre duas cargas puntiformes.

F = k · |q₁q₂| / r²

Onde:

- F = módulo da força elétrica (N);
- q₁ = primeira carga elétrica (C);
- q₂ = segunda carga elétrica (C);
- r = distância entre as cargas (m);
- k = constante eletrostática.

No vácuo:

k ≈ 8,99 × 10⁹ N·m²/C²

---

# 6. O que a Lei de Coulomb nos mostra?

A força elétrica é diretamente proporcional ao produto dos módulos das cargas:

F ∝ |q₁q₂|

e inversamente proporcional ao quadrado da distância:

F ∝ 1/r²

Portanto:

- aumentar as cargas aumenta a força;
- aumentar a distância diminui a força;
- a distância aparece elevada ao quadrado.

---

# 7. Influência da distância

Como:

F ∝ 1/r²

se dobrarmos a distância:

r → 2r

teremos:

F' = F/4

Se triplicarmos a distância:

r → 3r

teremos:

F' = F/9

Assim, a força elétrica diminui rapidamente com o aumento da distância.

---

# 8. Direção e sentido da força elétrica

A força elétrica atua ao longo da linha que une as duas cargas.

### Mesmo sinal

As forças apontam para sentidos que afastam as cargas:

**REPULSÃO**

### Sinais opostos

As forças apontam para sentidos que aproximam as cargas:

**ATRAÇÃO**

---

# 9. Lei de Coulomb e 3ª Lei de Newton

As duas cargas exercem forças uma sobre a outra.

Pela 3ª Lei de Newton:

F₁₂ = -F₂₁

Portanto:

|F₁₂| = |F₂₁|

As forças possuem:

- mesmo módulo;
- mesma direção;
- sentidos opostos.

> Uma carga não exerce uma força "maior" sobre a outra apenas por possuir maior carga ou maior massa.

---

# 10. Conversão de unidades

Antes de utilizar a Lei de Coulomb, todas as grandezas devem estar compatíveis com o Sistema Internacional.

### Distância

1 mm = 10⁻³ m

1 cm = 10⁻² m

1 km = 10³ m

### Carga

1 μC = 10⁻⁶ C

1 nC = 10⁻⁹ C

1 pC = 10⁻¹² C

> Atenção: utilizar centímetros, milímetros ou microcoulombs diretamente na fórmula sem conversão produz resultados incorretos.

---

# 11. Ambiente de desenvolvimento — Google Colab

Nesta aula utilizamos o **Google Colab** para executar programas em Python diretamente no navegador.

O Colab permite:

- executar código Python;
- desenvolver cálculos científicos;
- salvar notebooks;
- integrar arquivos ao Google Drive;
- testar diferentes situações físicas.

---

# 12. Hands On — Calculadora da Lei de Coulomb

Foi desenvolvida uma calculadora em Python para determinar a força eletrostática entre duas cargas puntiformes.

### Entradas

- carga q₁;
- carga q₂;
- distância r.

### Processamento

F = k · |q₁q₂| / r²

### Saída

- força eletrostática em Newtons.

---

## Exemplo em Python

```python
# Calculadora da Lei de Coulomb

k = 8.99e9

q1 = float(input("Digite a carga q1 em Coulomb: "))
q2 = float(input("Digite a carga q2 em Coulomb: "))
r = float(input("Digite a distância entre as cargas em metros: "))

F = k * abs(q1 * q2) / (r ** 2)

print("Força eletrostática:")
print(F, "N")
