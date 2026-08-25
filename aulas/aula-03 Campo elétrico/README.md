# Aula 03 — Campo Elétrico

## Eletromagnetismo Aplicado

Nesta aula estudamos o conceito de **campo elétrico**, sua relação com a força elétrica e a Lei de Coulomb, sua representação vetorial e suas principais aplicações em Engenharia Elétrica.

---

## Objetivos da aula

Ao final da aula, o estudante deverá ser capaz de:

- compreender o conceito físico de campo elétrico;
- diferenciar força elétrica de campo elétrico;
- calcular o campo produzido por uma carga puntiforme;
- identificar direção e sentido do vetor campo elétrico;
- interpretar linhas de campo elétrico;
- aplicar o princípio da superposição;
- utilizar Python para calcular campos elétricos;
- reconhecer aplicações do campo elétrico na Engenharia Elétrica.

---

# 1. Por que introduzimos o campo elétrico?

Uma carga elétrica modifica as propriedades do espaço ao seu redor.

Essa modificação é descrita pelo **campo elétrico**.

A ideia fundamental pode ser representada por:

Carga fonte  
↓  
modifica o espaço  
↓  
Campo elétrico  
↓  
colocamos uma carga de prova  
↓  
Força elétrica

Portanto, o campo elétrico existe independentemente da presença de uma carga de prova.

---

# 2. Força elétrica × Campo elétrico

A força elétrica depende da carga colocada no campo:

F = q₀E

Já o campo elétrico caracteriza uma propriedade da região do espaço:

E = F/q₀

Onde:

- E = campo elétrico (N/C);
- F = força elétrica (N);
- q₀ = carga de prova (C).

> A carga fonte produz o campo elétrico. A carga de prova permite detectar seus efeitos.

---

# 3. Campo elétrico de uma carga puntiforme

Para uma carga puntiforme Q:

E = k|Q|/r²

Onde:

- E = módulo do campo elétrico;
- Q = carga fonte;
- r = distância entre a carga e o ponto analisado;
- k = constante eletrostática.

No vácuo:

k ≈ 8,99 × 10⁹ N·m²/C²

---

# 4. Direção e sentido do campo elétrico

O campo elétrico é uma **grandeza vetorial**.

Portanto, possui:

- módulo;
- direção;
- sentido.

### Carga positiva

Para Q > 0:

**o campo elétrico aponta para fora da carga.**

### Carga negativa

Para Q < 0:

**o campo elétrico aponta em direção à carga.**

---

# 5. Linhas de campo elétrico

As linhas de campo são representações gráficas utilizadas para visualizar o comportamento do campo elétrico no espaço.

Principais características:

1. começam em cargas positivas;
2. terminam em cargas negativas;
3. a tangente à linha indica a direção do campo;
4. maior concentração de linhas representa campo mais intenso;
5. linhas de campo elétrico nunca se cruzam.

> As linhas são uma ferramenta de representação. Elas não existem fisicamente.

---

# 6. Por que as linhas de campo não podem se cruzar?

Em cada ponto do espaço existe uma única direção para o vetor campo elétrico resultante.

Se duas linhas se cruzassem, teríamos duas direções diferentes para o campo elétrico no mesmo ponto.

Isso não é fisicamente possível.

---

# 7. Princípio da Superposição

Quando existem várias cargas elétricas, cada carga produz seu próprio campo.

O campo elétrico resultante é obtido pela **soma vetorial** dos campos individuais:

E_resultante = E₁ + E₂ + E₃ + ... + Eₙ

Portanto, devemos considerar:

- módulo;
- direção;
- sentido;
- componentes vetoriais.

---

# 8. Hands On — Python

Nesta aula utilizamos Python para desenvolver uma **Calculadora de Campo Elétrico**.

O programa recebe:

- carga Q;
- distância r.

E calcula:

E = k|Q|/r²

Além do módulo, o programa pode identificar o sentido do campo:

- Q > 0 → campo aponta para longe da carga;
- Q < 0 → campo aponta em direção à carga.

### Exemplo básico

```python
k = 8.99e9

Q = float(input("Digite a carga Q em C: "))
r = float(input("Digite a distância em metros: "))

E = k * abs(Q) / (r ** 2)

print("Campo elétrico =", E, "N/C")

if Q > 0:
    print("O campo aponta para longe da carga.")
elif Q < 0:
    print("O campo aponta em direção à carga.")
else:
    print("A carga é nula.")
