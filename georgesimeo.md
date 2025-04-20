Ok, aqui está a tradução do terceiro artigo científico para o Português do Brasil.

---

**Serdica J. Computing 4 (2010), 19-28**

**Serdica**
**Journal of Computing**

Academia Búlgara de Ciências
Instituto de Matemática e Informática

**MODELAGEM MATEMÁTICA PARA O ESTUDO DE PROCESSOS MICROBIANOS – ALGUNS EXEMPLOS**

**V. Beschkov, T. Sapundzhiev, K. Petrov, E. Vasileva**

**RESUMO.** A modelagem matemática pode ter diferentes propósitos nas ciências da engenharia química e bioquímica. Um deles é confirmar ou rejeitar modelos cinéticos para certos processos, ou avaliar a importância de alguns fenômenos de transporte na taxa de reação química ou bioquímica líquida. No presente artigo, diferentes processos microbianos são considerados e modelados para avaliação de constantes cinéticas para processos em batelada e contínuos realizados por células microbianas livres e imobilizadas. Os exemplos práticos são do campo de tratamento de águas residuárias e biossíntese de produtos, como enzimas, ácido lático, ácido glucônico, etc.

Com o auxílio da modelagem matemática, a cinética e o tipo de inibição são especificados para a desnitrificação microbiana de águas residuárias e biodegradação de hidrocarbonetos halogenados. A importância das células livres e imobilizadas e sua contribuição separada para o processo microbiano geral também é avaliada para alguns processos fermentativos: produção de ácido glucônico, biodegradação de dicloroetano, fermentação lática e biodegradação de ácido monocloroacético.

**Sistema de Classificação de Computação ACM (1998):** G.1.7, G.1.8.
**Palavras-chave:** cinética microbiana, células livres e imobilizadas, modelagem matemática, desprendimento celular, avaliação de parâmetros.

---

**20 V. Beschkov, T. Sapundzhiev, K. Petrov, E. Vasileva**

**1. Avaliação da cinética bioquímica.** Os experimentos cinéticos tradicionais são realizados sob condições em batelada em reatores de tanque agitado a temperatura fixa, dependendo das células microbianas específicas. Os modelos matemáticos consistem em conjuntos de equações diferenciais ordinárias, envolvendo inibição, seja por substrato, ou por produtos com diferente número de parâmetros conhecidos e desconhecidos. Estes últimos devem ser avaliados.

Existem diferentes modelos cinéticos levando em conta a inibição. Incluindo diferentes modelos cinéticos, podemos estimar o mais apropriado usando modelagem matemática. Aqui estão alguns exemplos.

**1.1. Desnitrificação microbiana.** A desnitrificação é usada para marcar a redução de compostos de nitrogênio oxidados para nitrogênio gasoso. Como resultado da redução, diferentes produtos intermediários e finais são produzidos: nitrito (NO₂⁻), óxido nítrico (NO), óxido nitroso (N₂O), ou nitrogênio molecular (N₂), pelas seguintes etapas consecutivas:

NO₃⁻ → NO₂⁻ → NO (g) → N₂O (g) → N₂ (g)

Foi estabelecido que o processo é retardado em concentrações mais altas de nitrato, devido à inibição pelo substrato S (i.e., NO₃⁻) ou pelo produto P (NO₂⁻).

A avaliação da cinética do processo requer um certo modelo de inibição. Neste caso, o seguinte conjunto de equações diferenciais ordinárias foi resolvido:

```
dS/dt = -αμΧ
dP/dt = αμΧ – βxΡ
dX/dt = μΧ – βxΧ
```
(1)

com as condições iniciais apropriadas:

```
t = 0, S = S₀, P = 0, X = X₀.
```
(2)

Dois tipos de inibição por substrato foram verificados: a equação de Andrews [1], Eq. (3a), e a de Aiba et al. [2], Eq. (3b).

```
μ = μmax * S / (Ks + S + KiS²)
```
(3a)

---

**Modelagem Matemática para o Estudo de Processos Microbianos 21**

```
μ = μmax * (S / (Ks + S)) * exp(-K₂S)
```
(3b)

A inibição por produto foi descrita por:

```
μ = μmax * (S / (K₄ + S)) * (K₃ / (K₃ + P))
```
(4)

Parâmetros desconhecidos a serem determinados são: α, βx, K₂ (ou Ki) e K₃. Os restantes foram previamente determinados experimentalmente. O sistema (1-4) foi resolvido pelo simulador 20-sim [3, 4], acoplado a um procedimento de otimização de Nelder-Mead para avaliação de parâmetros cinéticos. Como função minimizada, adotou-se a soma dos quadrados das diferenças entre os valores experimentais e os calculados para a concentração de nitrato:

```
F = Σᵢ (Si,exp - Si,calc)² ,
```
(5)

para seis diferentes concentrações iniciais de nitrato com 7 pontos experimentais para cada experimento. A adequação do modelo foi testada pela dispersão dos parâmetros cinéticos avaliados para diferentes concentrações de substrato e outras condições, e pelo teste F. Foi mostrado que a inibição pelo substrato segue melhor o modelo de Aiba, Eq. (3b), do que o de Andrews. A comparação entre os dados experimentais e os previstos pelo modelo mostra que há uma concordância muito boa para a redução de nitrato e apenas qualitativa para a redução de nitrito:

*(Figura 1: Gráfico mostrando a concentração de N (mg dm⁻³) versus Tempo (h). Inclui dados experimentais e curvas do modelo para NO₃-N e NO₂-N. Legenda: NO₃-N, experimento (losango cheio); NO₂-N, experimento (círculo vazio); NO₂-N, modelo (linha pontilhada); curva NO₃-N, modelo (linha sólida))*

**Fig. 1.** Comparação do modelo e dos dados experimentais. Concentração inicial de NO₃⁻-N: 139.5 mg/l

---

**22 V. Beschkov, T. Sapundzhiev, K. Petrov, E. Vasileva**

**1.2. Produção bacteriana de ciclodextrina-glucano-transferase (CGT-ase).** A enzima ciclodextrina-glucano-transferase (CGTase) é produzida por diferentes bactérias. Usamos resultados experimentais para a cepa *Bacillus circulans* em condições de batelada [5] para avaliar a cinética microbiana. O sistema similar (1-3) de equações diferenciais com os modelos cinéticos foi testado pelo mesmo procedimento de avaliação, diferindo pela taxa de formação do produto (i.e., CGTase), Eq. (6):

```
dP/dt = α·μ·Χ + β·Χ
```
(6)

e os parâmetros do modelo pela soma dos mínimos quadrados das concentrações do produto. Neste caso, a inibição pelo substrato seguiu melhor o modelo de Andrews [6].

**1.3. Desalogenação por células microbianas fixadas a suporte sólido.** A modelagem matemática foi usada neste caso para estimar a contribuição das células imobilizadas e das livres desprendidas do suporte para a biodegradação geral de 1,2-dicloroetano [7] em processo contínuo:

DCE → íons cloreto + outros produtos

```
dX₁/dt = μX₁ + kimXim + D₁(X - X₁)
```
(7)

```
dXim/dt = μimXim - kimXim
```
(7a)

```
dS₁/dt = -r(X₁) – r(Xim) – βX₁ – βimXim + D₁(S – S₁)
```
(7b)

com as condições iniciais:

```
t = 0, X = X₁ = 0, Xim = X⁰im, S₁ = 0, P₁ = 0.
```
(7c)

A concentração total de biomassa na fase líquida X₁ deve-se ao vazamento celular e ao consequente crescimento microbiano. Teoricamente, a biodegradação do substrato poderia ser realizada tanto pelas células livres quanto pelas imobilizadas, conforme dado pelas Eqs. (7b, c). A contribuição das células livres depende do fator de vazamento kim. Quanto maior kim, maior a contribuição das células livres. Se kim = 0, não há vazamento celular e o processo é realizado apenas pelas células imobilizadas.

---

**Modelagem Matemática para o Estudo de Processos Microbianos 23**

**Tabela 1.** Os valores dos parâmetros estimados para um processo contínuo para concentrações iniciais de DCE de 0.5 mM e diferentes taxas de diluição para células fixadas a suporte sólido

| Parâmetro/Taxa de diluição, h⁻¹ | 2.65   | 5.9    | 7.35   |
| :------------------------------ | :----- | :----- | :----- |
| kim, m.h⁻¹                      | 0.0008 | 0      | 0      |
| µmax,im, h⁻¹                    | 0.26   | 0.17   | 0.29   |
| Soma dos quadrados (-)          | 0.007  | 0.006  | 0.008  |

O tratamento dos dados experimentais para 3 diferentes concentrações iniciais de DCE pela técnica descrita acima e minimizando a soma dos quadrados das concentrações do produto (i.e., cloreto) mostrou que praticamente não há vazamento de células e a biodegradação deveu-se apenas às células imobilizadas, cf. Tabela 1. Para referência, o kim estimado foi menor que 0.001.

**2. Processos microbianos com células encapsuladas (fenômenos de transporte e desprendimento celular).** Neste caso, as células são encapsuladas em géis, como alginato de cálcio, poliacrilamida, etc. Há uma resistência à transferência de massa para moléculas de substrato e produto nos poros do gel e membranas e, portanto, as taxas de bioconversão aparentes são menores do que para células livres [8]. A transferência de massa retardada devido à difusão molecular pode piorar a situação caso o produto seja um inibidor. Por outro lado, as células podem crescer dentro das partículas e formar perfis de concentração com acesso diferente à alimentação de substrato. A situação se torna mais complicada quando as células vazam da periferia da partícula para o caldo, continuando a crescer independentemente.

Todos esses efeitos podem ser estimados e conclusões sobre a natureza e contribuição das células imobilizadas e das livres podem ser tiradas usando modelos matemáticos adequados e dados experimentais apropriados, minimizando a soma dos mínimos quadrados. Para o caso de processo em batelada com partículas de forma definida (i.e., esférica), pode-se escrever o seguinte sistema de equações diferenciais parciais [9]:

```
∂cs/∂t = Ds * (∂²cs/∂r² + (2/r) * ∂cs/∂r) - k₁ * dX/dt
∂cp/∂t = Dp * (∂²cp/∂r² + (2/r) * ∂cp/∂r) + k₁ * dX/dt - k₂XCp
```
(8)

---

**24 V. Beschkov, T. Sapundzhiev, K. Petrov, E. Vasileva**

Com as seguintes condições iniciais e de contorno:

```
t = 0, cs = c₀; cp = 0; X = X₀
```
(8a)

```
r = 0, ∂ci/∂r = 0,
```
(8b)

```
r = R, Di(∂ci/∂r) = k(cis - ci∞),
```
(8c)

Para uma cultura em batelada, a variação da concentração de produto no caldo ao longo do tempo é dada pelas seguintes equações, com as condições iniciais associadas:

```
V * dcp,∞/dt = -ADP * (∂cp/∂r)|r=R + V * (YP/X * dX∞/dt - k₂X∞cp,∞)
```
(9)

```
V * dX∞/dt = Vμ∞X∞ + kimA [μimXim]|r=R
```
(10)

```
t = 0, X∞ = X⁰∞, cp = c⁰p,∞
```

A taxa do processo depende de diferentes fatores, como o coeficiente de transferência de massa na fase líquida k, a área interfacial A, as taxas específicas de crescimento microbiano na fase líquida μ∞ e dentro das partículas μim, o coeficiente de rendimento do produto YP/X, etc. Os índices "∞" denotam concentrações e quantidades na fase líquida, enquanto "im" denota quantidades relacionadas às partículas de gel. Consideraremos reações consecutivas de duas etapas envolvendo degradação do produto na segunda etapa:

S → P → produtos de degradação

A cinética de crescimento microbiano segue equações como as Eqs. (3a, b) e (4), levando em conta a inibição tanto pelo substrato quanto pelo produto.

O sistema (9-10) foi resolvido numericamente para cada caso prático separado por um esquema de diferenças implícitas acoplado ao algoritmo de Thomas para resolver o sistema resultante de equações algébricas lineares. Existem alguns exemplos abaixo.

**2.1. Biotransformação de glicose em ácido glucônico [9].** A diferença experimental entre o desempenho de células livres e imobilizadas é mostrada na Fig. 2. Foi mostrado que o produto da constante de taxa e a concentração inicial de células imobilizadas.

*(Figura 2: Gráfico mostrando a dinâmica da conversão de glicose em ácido glucônico observada em cultura livre e por células imobilizadas de Gluconobacter oxydans. η(-) vs Tempo (h). Legenda: ajuste do modelo (linha sólida), limites superior e inferior (linhas pontilhadas), pontos experimentais (círculos cheios). β = 0.1, C⁰G = 40 kg/m³)*

**Fig. 2.** Dinâmica da conversão de glicose em ácido glucônico observada em cultura livre e por células imobilizadas de *Gluconobacter oxydans*. O fator de vazamento (aqui β) é 0.1

---

**Modelagem Matemática para o Estudo de Processos Microbianos 25**

**Tabela 2**

| Glicose, kg m⁻³ | µmax,∞, h⁻¹   | µmax,im, h⁻¹  | k₁X⁰im, g dm⁻³ |
| :-------------- | :------------ | :------------ | :------------- |
| 40              | 0.31 ± 0.05   | 0.38 ± 0.04   | 21             |
| 90              | 0.30 ± 0.03   | 0.38 ± 0.03   | 22             |
| 180             | 0.34 ± 0.04   | 0.34 ± 0.05   | 24             |

k₁X⁰im foi muito estável para uma ampla faixa de concentrações iniciais de glicose (de 40 a 180 kgm⁻³) argumentando pela validade do modelo, cf. Tabela 2. Neste caso, a taxa máxima específica de crescimento microbiano para as células imobilizadas foi comparável (até um pouco maior) à das células livres.

**2.2. Fermentação lática [10].** A fermentação lática foi tratada como um estudo de caso para inibição por produto e seu impacto nas bactérias encapsuladas em partículas de gel. Os dados experimentais mostraram considerável vazamento celular e, portanto, rápida exaustão do biocatalisador. Essas observações foram quantificadas por um modelo similar ao das Eqs. (8-10). Alguns parâmetros avaliados pelo procedimento descrito acima são mostrados na Tabela 3.

Os valores de Φ²s = k₁μmax,imX⁰im·R²/(Dsc₀) são muito menores na primeira e na última corrida em comparação com as outras por causa da concentração muito baixa de biomassa dentro das partículas, devido à cultura não desenvolvida no início e à exaustão por causa do vazamento no final. A taxa específica de crescimento microbiano é muito baixa para compensar o vazamento celular, embora kim não seja muito alto.

**Tabela 3.** Os valores dos parâmetros cinéticos estimados para a fermentação lática

| Corrida No. | Φ²s, [-] | µmax,im, [h⁻¹] | kim, [-]  |
| :---------- | :------- | :------------- | :-------- |
| 1           | ~10⁻⁵    | 0.022          | 2.10⁻¹⁰   |
| 2           | 1.6      | 0.020          | 0.005     |
| 3           | 2.4      | 0.020          | 0.008     |
| 4           | 2.3      | 0.020          | 0.005     |
| 5           | 0.2      | 0.020          | 0.001     |


**2.3. Biodegradação de ácido monocloroacético [11].** Os experimentos sobre biodegradação de ácido monocloroacético (MCA) foram realizados com bactérias da cepa *Xanthobacter autotrophicus* GJ10, encapsuladas em gel de poliacrilamida. O mesmo conjunto de equações (8a-c) foi usado levando em conta a mineralização adicional do produto intermediário, por exemplo, ácido glicólico. As constantes de taxa (e.g., Φ²s e Φ²p), o fator de vazamento e a taxa máxima específica de crescimento microbiano nas partículas foram determinados minimizando a seguinte soma de quadrados, incluindo também os dados para o produto:

```
F = Σᵢ (Si,exp - Si,calc)² + Σᵢ (Pi,exp - Pi,calc)²
```
(11)

Alguns dos resultados para valores de parâmetros são mostrados na Tabela 4. A constante de taxa para a primeira reação varia com as diferentes corridas por causa do crescimento bacteriano dentro das células e pelo vazamento celular, representado por kim. A taxa máxima específica de crescimento microbiano nas partículas é constante, mas dez vezes menor do que a para células livres (0.155 h⁻¹). O fator de vazamento permanece constante para as corridas principais, tendendo a zero quando as partículas estão exauridas por causa do vazamento celular.

**Tabela 4.** Valores estimados dos parâmetros cinéticos para concentração inicial de MCA de 10 mM.

| Corrida No. | Φ²s, [-] | Φ²p, [-] | µmax,im, [h⁻¹] | kim, [-]  |
| :---------- | :------- | :------- | :------------- | :-------- |
| 1           | 2.14     | 1.10⁻⁵   | 0.023          | 4.2*10⁻⁴  |
| 2           | 10.9     | 1.10⁻⁴   | 0.023          | 0.015     |
| 3           | 17.36    | 5.10⁻⁵   | 0.023          | 0.015     |
| 4           | 8.84     | 5.10⁻⁵   | 0.023          | 0.015     |
| 5           | 8.647    | 1.10⁻⁵   | 0.023          | 0.015     |
| 6           | 1*10⁻⁶   | 1.10⁻⁵   | ~10⁻⁷          | 3.2*10⁻⁵  |

---

**REFERÊNCIAS**

[1] ANDREWS J. F. A mathematical model for the continuous culture of microorganisms utilizing inhibitory substrates. *Biotechnol. Bioeng.*, **10** (1968), 707–723.
[2] AIBA S., M. SHODA, M. NAGATANI. Kinetics of product inhibition in alcohol fermentation. *Biotechnol. Bioeng.* **67** (2000), 671–690.
[3] NATCHEVA M., V. BESCHKOV, TS. SAPUNDZHIEV. Mathematical modelling of thermophilic denitrification by bacterial consortium under anaerobic conditions. *Res. J. Chem. Environ.*, **9** (2005), 34–37.
[4] 20-sim 3.4, Controllab Products B. V., Enschede, The Netherlands. http://www.20sim.com
[5] VASSILEVA A., N. BURHAN, V. BESCHKOV, D. SPASOVA, S. RADOEVSKA, V. IVANOVA. Cyclodextrin Glucanotransferase Production by Free and Immobilised Cells of Bacillus circulans ATCC 21783. *Process Biochemistry*, **38** (2003), 1585–1591.
[6] BURHAN N., TS. SAPUNDZHIEV, V. BESCHKOV. Mathematical modeling of cyclodextrin-glucano-transferase production by batch cultivation. *Biochem. Eng. Journal*, **24** (2005), 73–77.
[7] MILEVA A., TS. SAPUNDZHIEV, V. BESCHKOV. Modelling 1,2-dichloroethane biodegradation by Klebsiella oxytoca VA 8391 immobilized on granulated activated carbon. *Bioproc. Biosys. Eng.*, **31** (2008), 75–85.
[8] DE BACKER L., R. G. WILLAERT, G. V. BARON. In: Immobilised living cell systems,modelling and experimental methods,(Eds R.G. Willaert, G.V. Baron, L. De Backer), J. Chichester, Wiley and Sons, 1996, 47–66.
[9] BESCHKOV V., S. VELIZAROV, T. GEORGIEVA. Simultaneous intraparticle diffusion, reaction and aerobic cell growth in a spherical gel biocatalysts: model and experiment. *Bulg. Chem. Commun.*, **31** (1999) 521–535.
[10] PETROV K. K., D. S. YANKOV, V. N. BESCHKOV. Lactic acid fermentation by cells of Lactobacillus rhamnosus immobilized in polyacrylamide gel. *World J. Microbiol. Biotechnol.*, **22** (2006), 337–345.
[11] VASILEVA Ε. Κ., Κ. Κ. PETROV, V. N. BESCHKOV. Modelling of monochloracetic acid biodegradation by immobilized cells of Xanthobacter autotrophicus GJ10. *Bulg. Chem. Commun.* (in press).

Instituto de Engenharia Química
Academia Búlgara de Ciências
1113 Sofia, Bulgária
e-mail: bioreac@bas.bg
e-mail: iihts@bas.bg
e-mail: kaloian04@yahoo.com
e-mail: evgeniavaslieva@yahoo.com

Recebido em 2 de novembro de 2009
Aceito final em 4 de fevereiro de 2010

---