# Eletromagnetismo Aplicado

### Engenharia Elétrica

Bem-vindo ao repositório da disciplina **Eletromagnetismo Aplicado**.

Este espaço reúne os materiais utilizados ao longo da disciplina, incluindo
**aulas, exercícios, códigos, atividades práticas, materiais complementares
e projetos aplicados à Engenharia Elétrica**.

---

## Sobre a disciplina

O Eletromagnetismo constitui uma das bases fundamentais da Engenharia Elétrica.

Ao longo da disciplina, estudaremos desde os fenômenos associados às
**cargas elétricas e campos elétricos** até campos magnéticos, indução
eletromagnética e as Equações de Maxwell.

A abordagem busca integrar:

**Fundamentos físicos + Modelagem matemática + Computação + Aplicações em Engenharia**

---

## Conteúdos da Disciplina

Ao longo do semestre serão estudados:

- Carga elétrica e propriedades da carga;
- Lei de Coulomb;
- Campo elétrico;
- Linhas de campo elétrico;
- Princípio da superposição;
- Fluxo elétrico;
- Lei de Gauss;
- Potencial elétrico;
- Energia potencial elétrica;
- Condutores e dielétricos;
- Capacitância;
- Campo magnético;
- Força magnética;
- Lei de Biot-Savart;
- Lei de Ampère;
- Indução eletromagnética;
- Lei de Faraday;
- Lei de Lenz;
- Equações de Maxwell;
- Ondas eletromagnéticas;
- Aplicações do eletromagnetismo na Engenharia.

---

# Aulas

## Aula 01 — Introdução ao Eletromagnetismo

Fundamentos da disciplina, grandezas físicas, sistemas de unidades,
análise vetorial e conceitos necessários para o estudo do eletromagnetismo.

[Acessar materiais da Aula 01](./aulas/)

---

## Aula 02 — Carga Elétrica e Campo Elétrico

### Conteúdos

- Carga elétrica;
- Quantização da carga;
- Conservação da carga;
- Interação entre cargas;
- Lei de Coulomb;
- Força elétrica;
- Conceito de campo elétrico;
- Campo produzido por cargas puntiformes;
- Direção e sentido do campo;
- Linhas de campo elétrico;
- Princípio da superposição;
- Aplicações em Engenharia.

[Acessar Aula 02](./aulas/aula-02-carga-eletrica-campo-eletrico/)

---

## Próximas aulas

Os materiais das próximas aulas serão disponibilizados progressivamente
ao longo do semestre.

---

# Atividades Práticas

Durante a disciplina serão desenvolvidas atividades envolvendo:

- resolução de problemas;
- interpretação física dos fenômenos;
- modelagem matemática;
- programação aplicada ao Eletromagnetismo;
- simulações computacionais;
- aplicações em Engenharia Elétrica.

---

# Python aplicado ao Eletromagnetismo

Alguns problemas estudados na disciplina também serão implementados
computacionalmente.

Exemplo de cálculo do campo elétrico produzido por uma carga puntiforme:

```python
k = 8.99e9

Q = float(input("Digite a carga Q em C: "))
r = float(input("Digite a distância em metros: "))

E = k * abs(Q) / r**2

print("Campo elétrico =", E, "N/C")

if Q > 0:
    print("Campo direcionado para longe da carga.")
else:
    print("Campo direcionado em direção à carga.")
