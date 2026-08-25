# Aulas — Eletromagnetismo Aplicado

Repositório de materiais, conteúdos, atividades e códigos desenvolvidos nas aulas da disciplina de **Eletromagnetismo Aplicado**.

**Curso:** Engenharia Elétrica — 5º semestre  
**Professora:** Karla Roberto Sartin

---

## Organização das aulas

### Aula 01 — Introdução e Análise Vetorial

📁 [`aula-01-introducao-analise-vetorial`](./aula-01-introducao-analise-vetorial/)

**Conteúdos:**

- introdução ao Eletromagnetismo;
- grandezas escalares e vetoriais;
- representação de vetores;
- componentes cartesianas;
- módulo, direção e sentido;
- operações com vetores;
- aplicações da análise vetorial ao Eletromagnetismo.

---

### Aula 02 — Carga Elétrica e Lei de Coulomb

📁 [`aula-02-carga-eletrica-campo-eletrico`](./aula-02-carga-eletrica-campo-eletrico/)

**Conteúdos:**

- conceito de carga elétrica;
- cargas positivas e negativas;
- propriedades da carga elétrica;
- conservação da carga;
- quantização da carga;
- interação entre cargas elétricas;
- atração e repulsão;
- Lei de Coulomb;
- influência da distância sobre a força elétrica;
- relação com as Leis de Newton;
- corrente elétrica e quantidade de carga.

**Prática computacional:**

- Google Colab;
- calculadora da Lei de Coulomb em Python;
- conversão automática de unidades;
- cálculo da força eletrostática;
- cálculo da distância entre cargas.

---

### Aula 03 — Campo Elétrico

📁 [`aula-03 Campo elétrico`](./aula-03%20Campo%20elétrico/)

**Conteúdos:**

- conceito de campo elétrico;
- força elétrica × campo elétrico;
- campo produzido por uma carga puntiforme;
- direção e sentido do campo elétrico;
- linhas de campo;
- princípio da superposição;
- campo elétrico resultante;
- aplicações em Engenharia Elétrica.

**Prática computacional:**

- calculadora de campo elétrico em Python;
- análise do módulo do campo;
- identificação do sentido do campo em função do sinal da carga.

---

### Aula 04 — Fluxo Elétrico e Lei de Gauss

📁 `aula-04-fluxo-eletrico-lei-de-gauss`

**Conteúdos:**

- revisão de campo elétrico;
- conceito de fluxo elétrico;
- vetor área e vetor normal;
- fluxo através de superfícies abertas;
- superfícies fechadas;
- Lei de Gauss;
- carga líquida encerrada;
- permissividade elétrica do vácuo;
- superfície gaussiana;
- importância da simetria.

**Aplicações da Lei de Gauss:**

- carga puntiforme — simetria esférica;
- esfera carregada — simetria esférica;
- fio muito longo — simetria cilíndrica;
- plano muito extenso — simetria planar;
- escolha da superfície gaussiana.

**Relação fundamental:**

\[
\boxed{
\Phi_E =
\oint_S \vec{E}\cdot d\vec{A}
=
\frac{Q_{\mathrm{int}}}{\varepsilon_0}
}
\]

> A Lei de Gauss é válida para qualquer superfície fechada.  
> A **simetria** é o que permite utilizá-la de forma eficiente para calcular o campo elétrico.

---

## Progressão conceitual

A sequência das aulas foi estruturada para construir gradualmente os conceitos do Eletromagnetismo:

```text
ANÁLISE VETORIAL
       ↓
CARGA ELÉTRICA
       ↓
FORÇA ELÉTRICA
       ↓
LEI DE COULOMB
       ↓
CAMPO ELÉTRICO
       ↓
FLUXO ELÉTRICO
       ↓
LEI DE GAUSS
       ↓
APLICAÇÕES EM ENGENHARIA ELÉTRICA
