Ok, aqui está a tradução do segundo artigo científico para o Português do Brasil, mantendo a informação e estrutura originais.

---

**Applied Mathematical Modelling 108 (2022) 205-219**

**Conteúdo disponível em ScienceDirect**

**Applied Mathematical Modelling**

**página inicial da revista: www.elsevier.com/locate/apm**

**Modelagem e identificação de parâmetros da fermentação microbiana em batelada sob perturbações ambientais**

**Jinggui Gaoª,*, Enmin Fengᵇ, Weihai Zhangᶜ**

ª Faculdade de matemática e ciência de sistemas, Universidade de Ciência e Tecnologia de Shandong, 266590, China
ᵇ Escola de Ciência Matemática, Universidade de Tecnologia de Dalian, Dalian, Liaoning 116024, China
ᶜ Faculdade de Engenharia Elétrica e Automação, Universidade de Ciência e Tecnologia de Shandong, 266590, China

**INFORMAÇÕES DO ARTIGO**

*Histórico do artigo:*
Recebido em 17 de outubro de 2021
Revisado em 18 de março de 2022
Aceito em 21 de março de 2022
Disponível online em 28 de março de 2022

*Palavras-chave:*
Cultura em batelada
Perturbação ambiental
Robustez biológica
Otimização multiobjetivo
Aproximação fuzzy

**RESUMO**

Este artigo considera a modelagem matemática e a identificação de parâmetros da bioconversão de glicerol em 1,3-Propanodiol na fermentação em batelada. Levando em conta a característica de estocasticidade genética inerente e as perturbações ambientais neste sistema bioquímico, um sistema diferencial estocástico com perturbação é proposto para descrever este processo de fermentação microbiana. Para garantir o refinamento do modelo e a robustez biológica simultaneamente, um modelo de identificação de parâmetros multiobjetivo é proposto. Para obter os parâmetros ótimos, o problema de otimização multiobjetivo é convertido em uma sequência de problemas de otimização de objetivo único. Em seguida, os problemas são adicionalmente aproximados a uma sequência dos problemas de otimização com restrições de desigualdade matricial linear com a ajuda da aproximação fuzzy T-S. Finalmente, os problemas de otimização foram resolvidos usando as técnicas de otimização de desigualdade matricial linear. Resultados numéricos mostram que o sistema dinâmico estocástico proposto é adequado para descrever este processo em batelada e nosso método proposto de identificação de parâmetros também é viável.
©2022 Elsevier Inc. Todos os direitos reservados.

**1. Introdução**

O 1,3-Propanodiol (1,3-PD) é uma matéria-prima química importante em medicamentos, cosméticos, alimentos e polímeros [1,2]. A síntese química e a conversão microbiana são dois processos principais de produção. A síntese química tem desvantagens óbvias de alta poluição, baixo rendimento e alto custo. Em comparação com a síntese química, a produção microbiana ganhou recentemente atenção popular e endosso científico em todo o mundo por sua alta produção, baixo custo e ausência de poluição.

No que diz respeito à tecnologia de fermentação biológica, existem três métodos de fermentação, incluindo cultura em batelada, cultura contínua e cultura alimentada em batelada. Entre essas técnicas, a operação em batelada pode obter os níveis mais altos de produtividade [3]. Em uma cultura em batelada típica de 1,3-PD, uma certa quantidade de glicerol e biomassa são adicionados ao recipiente, e então o processo de fermentação é interrompido após um período de fermentação. Muitas pesquisas mostraram que a biomassa inicial, a concentração inicial de glicerol e o tempo de fermentação são os principais fatores controláveis do rendimento do produto 1,3-PD durante a fermentação em batelada. Para tornar os esquemas de produção científicos e economicamente viáveis, é muito importante obter a estratégia de controle ótima. É uma abordagem viável obter a estratégia de controle ótima teórica por método matemático [4]. Portanto, o primeiro passo é formular o processo de fermentação em batelada por um modelo matemático para obter a estratégia teórica ótima. O processo de fermentação em batelada tem sido pesquisado extensivamente, incluindo modelagem de sistema não linear, otimização multiobjetivo e controle ótimo robusto. Em [5], uma nova abordagem de modelagem matemática foi proposta para descrever a cinética de produção de 1,3-PD em batelada por técnica de regressão não linear e dados de inibição por substrato/produto, e o modelo desenvolvido pode descrever adequadamente os dados experimentais. Ao introduzir perturbações paramétricas, o sistema cinético estocástico não linear foi proposto para descrever o processo de fermentação em batelada [6]. Nos últimos anos, vários modelos ótimos também foram propostos com base em diferentes perspectivas para esta fermentação microbiana. Por exemplo, com base na demanda industrial de maximização da produtividade e minimização do consumo, problemas de controle ótimo multiobjetivo foram estudados, e estratégias de controle apropriadas também foram obtidas para a fermentação de glicerol 1,3-PD [7]. Considerando a robustez biológica, problemas de controle ótimo robusto receberam muita atenção com base em diferentes índices de robustez biológica. A literatura [8] definiu sensibilidades da produtividade de 1,3-PD em relação ao atraso de tempo incerto como indicadores de robustez, e que é considerado como uma das funções objetivo ótimas. As literaturas [9,10] definiram a robustez biológica penalizando uma soma ponderada da expectativa e variância do desvio relativo com base em diferentes sistemas dinâmicos. Para o fator de atraso de tempo do sistema de fermentação, um sistema dinâmico chaveado não linear com atraso de tempo e o problema de controle ótimo foram estudados para o processo de bioconversão de glicerol em 1,3-PD [11]. Embora os resultados alcançados nas literaturas acima sejam interessantes, a estocasticidade genética inerente e a perturbação ambiental externa em redes biológicas não são consideradas nos trabalhos existentes.

De fato, uma rede biológica é incerta no sistema bioquímico em nanoescala [12]. Existem três tipos principais de perturbações de rede em redes biológicas [12]: variância microambiental, mudança macroambiental e variância genética. A variância microambiental também é chamada de ruído molecular estocástico, que frequentemente ocorre em qualquer rede biológica. A mudança macroambiental é a variação causada pelo ambiente externo, como temperatura, alimento, etc. A variância genética, que também é chamada de perturbação estocástica intrínseca, é uma mutação hereditária de uma molécula de DNA do genoma, que pode afetar o crescimento e desenvolvimento das células biológicas. Tanto a variância microambiental quanto a mudança macroambiental são perturbações ambientais não hereditárias, mas a variância genética é uma estocasticidade inerente hereditária. Para descrever com precisão os sistemas biológicos, a consideração das perturbações da rede biológica é necessária para formular o sistema biológico [4]. Problemas de controle multiobjetivo com consideração de perturbações da rede biológica para sistemas biológicos não lineares foram extensivamente estudados por muitos pesquisadores [13,14]. Diferente dos trabalhos anteriores, a robustez ótima é considerada neste artigo. Até onde sei, poucos trabalhos foram desenvolvidos para modelar este processo de fermentação em batelada envolvendo estocasticidade intrínseca e perturbação ambiental externa.

Neste artigo, um novo modelo matemático é proposto para formular este processo em batelada, onde a estocasticidade genética inerente é introduzida por perturbação de parâmetros, que é uma técnica popular em modelagem estocástica de populações [4], e as perturbações ambientais não hereditárias também são descritas introduzindo processos estocásticos não antecipativos. Então, um sistema diferencial estocástico com parâmetros cinéticos desconhecidos, que é impulsionado por movimento Browniano de cinco dimensões, é proposto para descrever esta cultura microbiana em batelada. Neste artigo, os parâmetros cinéticos desconhecidos serão identificados de modo a determinar o modelo do sistema biológico com base em dados experimentais reais e robustez biológica.

Robustez biológica é a capacidade de manter traços fenotípicos de redes biológicas face a perturbações aleatórias, que é uma das características fundamentais dos sistemas biológicos [15]. Este ponto de vista tem sido amplamente aceito por especialistas em biologia [15]. A robustez de um traço fenotípico de redes biológicas pode ser medida pela variação máxima das saídas do sistema face a uma perturbação específica.

Para melhorar o refinamento do modelo e manter a robustez de um traço fenotípico de redes biológicas, o sistema estocástico não linear com parâmetros cinéticos desconhecidos deve ser determinado para garantir simultaneamente o requisito de robustez ótima e o requisito de erro mínimo. Para obter os parâmetros cinéticos ótimos, um modelo de identificação de parâmetros multiobjetivo é proposto. Em seguida, uma sequência de problemas de otimização de objetivo único com restrições de desigualdade de Hamilton-Jacobi (restrições-HJI) são propostas para aproximar o modelo de identificação de parâmetros multiobjetivo neste artigo. No entanto, nos modelos de otimização acima, as soluções numéricas ou analíticas ótimas são difíceis de serem obtidas devido à alta não linearidade.

Existem várias maneiras diferentes de fazer uma linearização local para um sistema não linear, onde uma técnica popular é o sistema fuzzy T-S. Desde o artigo clássico de Takagi e Sugeno [16], o sistema fuzzy T-S ganhou reconhecimento e foi intensivamente aplicado em matemática e ciências da computação [14]. Neste artigo, empregando o sistema fuzzy T-S para aproximar o sistema estocástico não linear, uma sequência de problemas ótimos com restrições-HJI é aproximada a problemas de otimização com restrições de desigualdade matricial linear (restrições-LMI). Então, um algoritmo de otimização é proposto para resolver o problema de otimização com restrições-LMI. Simulações numéricas indicam que o sistema dinâmico estocástico proposto é apropriado para descrever o processo de fermentação microbiana em batelada. A fermentação microbiana de glicerol para 1,3-Propanodiol tem sido recentemente estudada extensivamente devido à sua alta produção, baixo custo e ausência de poluição. Comparado às literaturas existentes, as principais contribuições deste artigo são as seguintes: (i) Considerando a incerteza do processo de fermentação microbiana, um novo método de modelagem matemática é proposto para descrever este processo, no qual a estocasticidade inerente hereditária é descrita por perturbação de parâmetros e as perturbações ambientais não hereditárias são descritas por processos estocásticos. (ii) Para obter os parâmetros dinâmicos ótimos e o vetor de parâmetros de perturbação, a robustez ambiental é usada como um dos critérios para construir o problema de otimização multiobjetivo. (iii) Para este processo de fermentação microbiana, alguns novos resultados sobre a distribuição de perturbações ambientais aleatórias são obtidos.

O restante deste artigo está organizado da seguinte forma. A Seção 2 propõe um sistema dinâmico estocástico não linear da bioconversão de glicerol em 1,3-PD em cultura em batelada. Para obter os parâmetros ótimos, um modelo de identificação de parâmetros multiobjetivo é apresentado na Seção 3, e um algoritmo de otimização também é desenvolvido com base na otimização com restrições-LMI nesta seção. A Seção 4 apresenta simulações numéricas. As conclusões são apresentadas na Seção 5.

**2. Sistema dinâmico estocástico não linear de cultura em batelada**

O processo de fermentação da bioconversão de glicerol em 1,3-PD tem sido amplamente investigado. Sob condições anaeróbicas a 37 °C e pH 7.0, os balanços de massa de biomassa, substrato e produtos na cultura em batelada podem ser escritos da seguinte forma (ver Wang et al. [6]):

```
ẋ(t) = f(x(t), p), t ∈ [0, tf],
x(0) = x0.
```
(1)

Aqui, x(t) = (x₁(t), x₂(t), . . ., x₅(t))ᵀ é o vetor de estado, onde os componentes do vetor de estado denotam respectivamente as concentrações de biomassa, glicerol extracelular, 1,3-PD extracelular, acetato e etanol no tempo t no reator; x₀ denota o estado inicial.

```
f(x(t), p) = [ μx₁(t); -q₂x₁(t); q₃x₁(t); q₄x₁(t); q₅x₁(t) ]
```

onde a taxa específica de crescimento das células μ, a taxa específica de consumo do substrato glicerol q₂ e as taxas específicas de formação qi, i = 3, 4, 5 de 1,3-PD, acetato e etanol podem ser expressas pelas seguintes equações:

```
μ = μm * (x₂ / (x₂ + ks)) * Π(i=2 a 5) (1 - (xi(t) / x̄i(t)))
q₂ = m₂ + μ / Y₂
qi = mᵢ + μYi, i = 3, 4, 5.
```

Aqui, µm = 0.67 e ks = 0.28 [17], que são chamadas de taxa máxima específica de crescimento e constante de saturação de Monod; m₂ e Y₂ são o termo de manutenção do consumo de substrato e o rendimento máximo de crescimento, respectivamente; mᵢ e Yᵢ, i = 3, 4, 5, são os termos de manutenção e os rendimentos máximos de crescimento de 1,3-PD, acetato e etanol sob condições limitadas por substrato; Denote o vetor de parâmetros do sistema como p := (m₂, Y₂, m₃, Y₃, m₄, Y₄, m₅, Y₅)ᵀ ∈ ℝ⁸; x̄ⱼ, j = 1, ..., 5 são os valores críticos dos estados do sistema [11]; Seja S₀ = {x(t) ∈ ℝ⁵|x₁(t) ∈ [0.01, x̄₁], xᵢ(t) ∈ [0, x̄ᵢ], i = 2, 3, 4, 5} a faixa admissível dos estados do sistema; [0, tf] é o intervalo de tempo desta fermentação em batelada. Seja D = Π(i=1 a 8)[pᵢ, p̄ᵢ] o conjunto admissível do vetor de parâmetros, onde pᵢ e p̄ᵢ são os valores críticos inferior e superior, respectivamente. Seja (Ω, F, {Ft}t≥0, P) um espaço de probabilidade completo, onde F é uma σ-álgebra de subconjuntos de Ω com uma filtração {Ft}t≥0 satisfazendo as condições usuais. Denote o espaço de processos estocásticos não antecipativos limitados como L²F([0, tf], ℝ⁵).

De fato, as redes biológicas são sempre incertas no nível nanoscópico [12]. Variância microambiental, mudança macroambiental e variância genética são três perturbações principais na rede biológica [12]. A variância microambiental descreve as flutuações estocásticas da concentração de moléculas biológicas. A mudança macroambiental mostra a variação no ambiente externo. A variância genética é uma mutação hereditária de uma molécula de DNA do genoma, que também é chamada de perturbação estocástica intrínseca. Tanto a variância microambiental quanto a mudança macroambiental são perturbações ambientais não hereditárias, mas a variância genética são perturbações aleatórias inerentes hereditárias. Para descobrir a natureza precisa da cultura em batelada de glicerol, é muito necessário considerar as perturbações do sistema biológico.

A variância genética neste sistema bioquímico é uma estocasticidade inerente hereditária, que pode ser descrita por perturbação de parâmetros [6]. Neste artigo, assumimos que o rendimento máximo de crescimento, o requisito de manutenção da formação do produto e o requisito de manutenção do consumo de substrato são estocasticamente incertos in vivo. Assim, os parâmetros podem ser perturbados estocasticamente da seguinte forma:

mᵢ → mᵢ + Δmᵢnᵢ(t), Yᵢ → Yᵢ + ΔYᵢnᵢ(t), i = 2, 3, 4, 5. (2)

Na Eq. (2), Δmᵢ e ΔYᵢ são os desvios padrão do parâmetro cinético, que são partes determinísticas; Seja Δp := (Δm₂, ΔY₂, Δm₃, ΔY₃, Δm₄, ΔY₄, Δm₅, ΔY₅)ᵀ ∈ ℝ⁸; nᵢ(t) é um ruído branco Gaussiano com média zero e variância unitária, que denota a i-ésima fonte de flutuação aleatória.

Durante o processo de fermentação em batelada de glicerol, o sistema de fermentação microbiana também sofre de perturbações ambientais não hereditárias (como variância microambiental e mudança macroambiental), que podem ser descritas por processos estocásticos v(t) ∈ L²F([0, tf], ℝ⁵).

Então, o modelo matemático da bioconversão de glicerol em 1,3-PD na fermentação em batelada sob perturbações ambientais pode ser descrito como

```
dx(t) = b(p, x(t))dt + σ(Δp, p, x(t))dw(t), t ∈ [0, tf],
x(0) = x₀,
```
(3)

onde b(p, x(t)) = f(p, x(t)) + v(t), σ(Δp, p, x(t)) = (0, σ₂(x(t)), σ₃(x(t)), σ₄(x(t)), σ₅(x(t)))ᵀ, 0 = (0)₅ₓ₁, σk(x(t)) = Mk*g(p, x(t)), dw = (dw₁, dw₂, dw₃, dw₄, dw₅)ᵀ. Aqui, g(p, x(t)) = (x₁, μx₁/Y₂, μx₁)ᵀ e Mk pode ser escrito como

*(Matrizes M2, M3, M4, M5 são apresentadas aqui)*

Para discutir a existência e unicidade da solução para o sistema estocástico (3), para dados Δp, p, primeiramente discutimos as propriedades da função vetorial b(p, x) e da função matricial σ(Δp, p, x) definidas em (3).

**Propriedade 2.1.** Para dados Δp, p, a função vetorial b(p, x) e a função matricial σ(Δp, p, x) definidas por (3) são funções mensuráveis para x ∈ S₀, e existem constantes K e C tais que as seguintes condições se mantêm:
(i) condição de Lipschitz uniforme
||b(p, x¹) – b(p, x²)|| + ||σ(Δp, p, x¹) – σ(Δp, p, x²)|| ≤ K||x¹ – x²||, ∀x¹, x² ∈ S₀
(ii) condição de crescimento
||b(p, x)|| + ||σ(Δp, p, x)|| ≤ C(1 + ||x||), ∀x ∈ S₀,
onde ||·|| denota a norma Euclidiana.

**Prova.** A prova da função mensurável é óbvia a partir da continuidade das funções.
Para a função vetorial b(p, x) = f(p, x) + v, onde v é um vetor limitado, similar ao Teorema 2 em Wang et al. [6], podemos provar facilmente que existem constantes K₁ e C₁ tais que as seguintes condições se mantêm:
||b(p, x¹) – b(p, x²)|| ≤ K₁||x¹ – x²||, ∀x¹, x² ∈ S₀
||b(p, x)|| ≤ C₁(1 + ||x||), ∀x ∈ S₀
Para a função matricial σ(Δp, p, x), com base no Teorema do Valor Médio Diferencial, para quaisquer x¹, x² ∈ S₀, temos
||σ(Δp, p, x¹) – σ(Δp, p, x²)|| = √Σ(k=2 a 5) ||Mk*g(x¹) – Mk*g(x²)||² ≤ √Σ(k=2 a 5) ||Mk||²||g(x¹) – g(x²)||²
≤ √Σ(k=2 a 5) ||Mk||²||Jg(x¹ + δ(x² – x¹))||²||x¹ – x²||² onde 0 < δ < 1, Jg(p, x¹ + δ(x¹ – x²)) denota o Jacobiano de g(p, x) em x¹ + δ(x¹ – x²). Como g(p, x) é continuamente diferenciável em S₀ e S₀ é um conjunto compacto, seja G = max(x∈S₀) ||Jg(p, x)||. Então, temos
||σ(Δp, p, x¹) – σ(Δp, p, x²)|| ≤ K₂||x¹ – x²|| (K₂ = G√Σ(k=2 a 5) ||Mk||²)
Similarmente, para qualquer x ∈ S₀, temos
||σ(Δp, p, x)|| = √Σ(k=2 a 5) ||Mk*g(x)||² ≤ √Σ(k=2 a 5) ||Mk||²||g(x)||² ≤ √Σ(k=2 a 5) ||Mk||²(1 + μm/Y₂² + μm²)²||x||²
Então, temos
||σ(Δp, p, x)|| ≤ C₂(1 + ||x||) (C₂ = √Σ(k=2 a 5) ||Mk||²(1 + μm/Y₂² + μm²)²)
Portanto, fazendo K = K₁ + K₂; C = C₁ + C₂, podemos obter.
||b(p, x¹) – b(p, x²)|| + ||σ(Δp, p, x¹) – σ(Δp, p, x²)|| ≤ K||x¹ – x²||
||b(p, x)|| + ||σ(Δp, p, x)|| ≤ C(1 + ||x||)

Com base na Propriedade 2.1 e no Teorema 5.2.1 no Capítulo 5 em Øksendal [18], podemos obter o seguinte teorema.

**Teorema 2.1 (Existência e unicidade).** Para dada a função b(p, x(t)) e σ(Δp, p, x(t)), o sistema (3) tem uma única solução t-contínua x(t) satisfazendo a condição inicial x₀ em [0, tf].

**3. Problema de identificação de parâmetros e algoritmo**

A robustez biológica é a capacidade de manter traços fenotípicos de redes biológicas face a perturbações ambientais, que é uma das características fundamentais dos sistemas biológicos. Portanto, é bastante natural que a robustez seja um dos critérios para selecionar o modelo matemático ótimo [19]. Então, modelos matemáticos teóricos de redes biológicas não só devem ser capazes de rastrear dados experimentais reais, mas também ser robustos.

Para determinar o modelo matemático teórico, um vetor de parâmetros adequado deve ser selecionado da faixa admissível D. Com base na discussão acima, sabemos que a robustez e a capacidade de rastrear dados experimentais reais devem ser usadas como dois critérios para determinar o ótimo entre modelos matemáticos candidatos. Portanto, nossa identificação de parâmetros é determinar o sistema dinâmico estocástico não linear selecionando um vetor de parâmetros adequado para atender ao requisito de robustez ótima e rastrear otimamente o experimental real. Um modelo de saída experimental impulsionado por dados experimentais fornecido da seguinte forma [20]:

dx*(t) = [Ar(t) + r(t)]dt, t ∈ [0, tf], (4)

onde x*(t) são dados de saída de estado experimental, Ar(t) é especificado previamente para gerar um comportamento desejado de acordo com os dados experimentais, e r(t) ∈ L²F([0, tf], ℝ⁵) descreve perturbações de saída.

Robustez biológica é a capacidade de manter traços fenotípicos de redes biológicas face a perturbações aleatórias [19]. Assim, a medição da robustez biológica pode ser definida como a variação das saídas do sistema face a uma perturbação específica. Os índices quantitativos de robustez biológica foram propostos e estudados extensivamente por muitos estudiosos [21,22]. De fato, os índices quantitativos de robustez nas literaturas acima são todos definidos por robustez de parâmetros. Diferente da literatura acima, o índice de robustez biológica neste artigo é descrito por perturbações ambientais.

Com base na definição de robustez em Flix e Barkoulas [12], o índice de medida de robustez biológica pode ser definido como

R(p) := max(r(t),v(t)∈L²F([0,tf],ℝ¹⁰)) [ E[∫(0 a tf) (x(t) – x*(t))ᵀ(x(t) – x*(t))dt] / E[∫(0 a tf) [vᵀ(t)v(t) + rᵀ(t)r(t)]dt] ] (5)

onde x(t) e x*(t) são as saídas do sistema teórico em (3) e a saída de teste, respectivamente, e E denota a esperança. Da Eq. (5), sabemos que quanto menor o valor da equação R(p), mais robusto é o sistema. Portanto, esperamos encontrar um vetor de parâmetros para minimizar R(p).

O objetivo deste artigo é determinar o sistema dinâmico estocástico não linear selecionando um vetor de parâmetros adequado para atender ao requisito de robustez ótima e ao requisito de erro mínimo. Portanto, temos que otimizar os dois problemas de otimização a seguir simultaneamente para o sistema dinâmico estocástico não linear (3):

min(p∈D) R(p) (6)

e

min(p∈D) E ∫(0 a tf) (x(t) – x*(t))ᵀ(x(t) – x*(t))dt (7)

Portanto, o modelo de identificação de parâmetros multiobjetivo (MPIP) pode ser descrito como:

(MPIP): min(p∈D) [ R(p); E∫(0 a tf) (x(t) – x*(t))ᵀ(x(t) – x*(t))dt ] (8)
s.t. Eq.(3)

Até agora, existem duas abordagens gerais para resolver problemas multiobjetivo [23]. Uma é transformar as funções multiobjetivo em uma função objetivo única pelo método de ponderação e método de restrição, e então alcançar a solução da função multiobjetivo. A segunda abordagem geral é determinar diretamente o conjunto de soluções ótimas de Pareto da otimização multiobjetivo. Diferente das abordagens gerais acima, o vetor de parâmetros ótimo em (MPIP) é obtido empregando o método de aproximação alternativa neste artigo. Assim, o sistema dinâmico estocástico não linear (3) pode ser reescrito como:

dx̄(t) = b̄(p, x̄(t))dt + σ̄(p, x̄(t))dw̄, (9)

onde b̄(p, x̄(t)) = f̄(p, x̄(t)) + v̄(t), σ̄(p, x̄(t)) = (0, σ̄₂(x̄(t)), σ̄₃(x̄(t)), σ̄₄(x̄(t)), σ̄₅(x̄(t)))ᵀ, 0 = (0)₅ₓ₁, σ̄k(x̄(t)) = M̄k*ḡ(p, x̄(t)), k = 2, 3, 4, 5. Aqui,

x̄(t) = [x(t); x*(t)], v̄(t) = [v(t); r(t)], M̄k = [Mk; 0], f̄(p, x̄(t)) = [f(p, x(t)); Ar(t)]
ḡ(p, x̄(t)) = g(p, x(t)),

Então, o Problema (MPIP) é equivalente ao seguinte:

(EPIP): min(p∈D) [ R(p); E∫(0 a tf) x̄ᵀ(t)Qx̄(t)dt ] (10)
s.t. Eq.(9)
onde Q = [-I I; -I I], I é matriz identidade.

Para alcançar a solução ótima no Problema (EPIP), realizamos duas etapas, o requisito de robustez ótima (6) é primeiramente transformado em uma sequência de questões com restrições-HJI para o sistema estocástico com entrada inicial zero, então, com base em uma abordagem subótima, o requisito de erro ótimo (7) também é transformado nos problemas subótimos com restrições-HJI.

Para o objetivo de robustez ótima (6), primeiramente fazemos γ = min(p∈D) R(p) e uma sequência decrescente {γⱼ}ⱼ≥₁ tal que γⱼ → γ quando j → ∞. Para qualquer γⱼ ∈ {γⱼ}ⱼ≥₁, temos γ ≤ γⱼ. Portanto, deve haver um conjunto Dⱼ ⊂ D, tal que para qualquer p ∈ Dⱼ,

max(v(t)∈L²F([0,tf],ℝ¹⁰)) [ E[∫(0 a tf) x̄ᵀ(t)Qx̄(t)dt] / E[∫(0 a tf) v̄ᵀ(t)v̄(t)dt] ] ≤ γⱼ (11)

Para obter o vetor de parâmetros de robustez ótimo p, fazemos γⱼ → γ até que nenhum parâmetro p exista em D tal que a Eq. (11) se mantenha.

**Teorema 3.1.** Para o sistema dinâmico estocástico em (9), se existe Dⱼ ⊂ D, tal que a seguinte HJI tem uma solução positiva V(x̄) para cada p ∈ Dⱼ

(∂V(x̄)/∂x̄)ᵀ * f̄(p, x̄, t) + ½ Σ(k=1 a 5) ḡᵀ(p, x̄, t)M̄kᵀ * (∂²V(x̄)/∂x̄²) * M̄k*ḡ(p, x̄, t) + (1/4γⱼ) * (∂V(x̄)/∂x̄)ᵀ * (∂V(x̄)/∂x̄) + x̄ᵀ(t)Qx̄(t) ≤ 0. (12)

Então, a Eq. (11) se mantém.

**Prova.** Para qualquer p ∈ Dⱼ,

max(v(t)∈L²F([0,tf],ℝ¹⁰)) [ E[∫(0 a tf) x̄ᵀ(t)Qx̄(t)dt] / E[∫(0 a tf) v̄ᵀ(t)v̄(t)dt] ] ≤ γⱼ

A fórmula acima é equivalente ao seguinte problema de otimização [24]

max(v(t)∈L²F([0,tf],ℝ¹⁰)) E ∫(0 a tf) (x̄ᵀ(t)Qx̄(t) – γⱼv̄ᵀ(t)v̄(t))dt ≤ 0 (13)

Seja J(γⱼ) = E ∫(0 a tf) (x̄ᵀ(t)Qx̄(t) – γⱼv̄ᵀ(t)v̄(t))dt;
J₀(γⱼ) Δ= max(v(t)∈L²F([0,tf],ℝ¹⁰)) J(γⱼ).

Então, a Eq. (13) pode ser convertida para o seguinte problema de otimização [24]

max(v(t)∈L²F([0,tf],ℝ¹⁰)) E ∫(0 a tf) (x̄ᵀ(t)Qx̄(t) – γⱼv̄ᵀ(t)v̄(t))dt; (14)
s.t. J₀(γⱼ) ≤ 0;

Seja V(x̄(t)) uma função de Lyapunov positiva com V(0) = 0 para o sistema (9). Então, temos

J(γⱼ) = E ∫(0 a tf) (x̄ᵀ(t)Qx̄(t) – γⱼv̄ᵀ(t)v̄(t))dt = -EV(x̄(tf)) + E ∫(0 a tf) (x̄ᵀ(t)Qx̄(t) – γⱼv̄ᵀ(t)v̄(t))dt + E ∫(0 a tf) dV(x̄(t)). (15)

Pelo Teorema 4.1.2 no Capítulo 4 em Øksendal [18], obtemos

dV(x̄(t)) = (∂V(x̄)/∂x̄)ᵀ * f̄(p, x̄, t)dt + (∂V(x̄)/∂x̄)ᵀ * v̄(t)dt + Σ(k=2 a 5) (∂V(x̄)/∂x̄)ᵀ * M̄k*ḡ(p, x̄, t)dwk + ½ Σ(k=2 a 5) ḡᵀ(p, x̄, t)M̄kᵀ * (∂²V(x̄)/∂x̄²) * M̄k*ḡ(p, x̄, t)dt. (16)

Substituindo (16) em (15), obtemos

J(γⱼ) = E ∫(0 a tf) (x̄ᵀ(t)Qx̄(t) – γⱼv̄ᵀ(t)v̄(t))dt
= -EV(x̄(tf)) + E ∫(0 a tf) [ x̄ᵀ(t)Qx̄(t) + (∂V(x̄)/∂x̄)ᵀ * f̄(p, x̄, t) + (1/4γⱼ) * (∂V(x̄)/∂x̄)ᵀ * (∂V(x̄)/∂x̄) - (√(γⱼ)v̄(t) - (1/2√(γⱼ)) * (∂V(x̄)/∂x̄))ᵀ * (√(γⱼ)v̄(t) - (1/2√(γⱼ)) * (∂V(x̄)/∂x̄)) + ½ Σ(k=2 a 5) ḡᵀ(p, x̄, t)M̄kᵀ * (∂²V(x̄)/∂x̄²) * M̄k*ḡ(p, x̄, t) ] dt. (17)

Então,
J₀(γⱼ) = max(v(t)∈L²F([0,tf],ℝ¹⁰)) J(γⱼ) = max(v(t)∈L²F([0,tf],ℝ¹⁰)) E ∫(0 a tf) (x̄ᵀ(t)Qx̄(t) – γⱼv̄ᵀ(t)v̄(t))dt
= -EV(x̄(tf)) + E ∫(0 a tf) [ x̄ᵀ(t)Qx̄(t) + (∂V(x̄)/∂x̄)ᵀ * f̄(p, x̄, t) + (1/4γⱼ) * (∂V(x̄)/∂x̄)ᵀ * (∂V(x̄)/∂x̄) + ½ Σ(k=2 a 5) ḡᵀ(p, x̄, t)M̄kᵀ * (∂²V(x̄)/∂x̄²) * M̄k*ḡ(p, x̄, t) ] dt.

Então, quando a desigualdade (12) se mantém, a seguinte desigualdade se mantém
J₀(γⱼ) ≤ 0.
□

Então, o requisito de erro mínimo em (7) também pode ser transformado nos problemas subótimos com restrições-HJI [25].

**Teorema 3.2.** O requisito de erro mínimo em (7) é aproximado ao seguinte problema de otimização

min(p∈D) EV(x̄(0))
s.t. (∂V(x̄)/∂x̄)ᵀ * f̄(p, x̄, t) + ½ Σ(k=2 a 5) ḡᵀ(p, x̄, t)M̄kᵀ * (∂²V(x̄)/∂x̄²) * M̄k*ḡ(p, x̄, t) + ¼ (∂V(x̄)/∂x̄)ᵀ * (∂V(x̄)/∂x̄) + x̄ᵀ(t)Q̄x̄(t) ≤ 0, (18)

onde V(x̄) é uma função de Lyapunov positiva do sistema estocástico não linear em (9).

**Prova.** Seja V(x̄) uma função de Lyapunov positiva para o sistema estocástico não linear em (9). Pelo fato

(∂V(x̄)/∂x̄)ᵀ * v̄(t) ≤ ¼ (∂V(x̄)/∂x̄)ᵀ * (∂V(x̄)/∂x̄) + v̄ᵀ(t)v̄(t). (19)

Então, obtemos

E ∫(0 a tf) x̄ᵀ(t)Q̄x̄(t)dt ≤ EV(x̄(0)) + E ∫(0 a tf) [ x̄ᵀ(t)Q̄x̄(t) + (∂V(x̄)/∂x̄)ᵀ * f̄(p, x̄, t) + ¼ (∂V(x̄)/∂x̄)ᵀ * (∂V(x̄)/∂x̄) + ½ Σ(k=2 a 5) ḡᵀ(p, x̄, t)M̄kᵀ * (∂²V(x̄)/∂x̄²) * M̄k*ḡ(p, x̄, t) + v̄ᵀ(t)v̄(t) ] dt. (20)

Além disso, se a HJI em (18) se mantém, então temos

E ∫(0 a tf) x̄ᵀ(t)Q̄x̄(t)dt ≤ EV(x̄(0)) + E ∫(0 a tf) v̄ᵀ(t)v̄(t)dt.

Como o último termo E ∫(0 a tf) v̄ᵀ(t)v̄(t)dt na desigualdade acima é independente da seleção de p, o requisito de erro do sistema estocástico (9) é aproximadamente equivalente a min(p∈D) EV(x̄(0)) com restrições-HJI. □

Então, o Problema (EPIP) é aproximado a uma sequência de Problemas {(EPIP(γⱼ))}ⱼ≥₁, onde (EPIP(γⱼ)) é definido como

(EPIP(γⱼ)): min(p∈D) J(p) := EV(x̄(0)) (21)
s. t. Eqs. (12), (18).

De fato, o Problema de otimização (EPIP(γⱼ)) é difícil de ser resolvido devido à não linearidade. Uma linearização local pelo método de interpolação fuzzy T-S é simples e fácil de superar essas dificuldades.
Primeiramente, damos as seguintes regras fuzzy:
Regra i: se X₁(t) é F₁ᵢ e . . . e X₅(t) é F₅ᵢ, então

dx(t) = (Aᵢ(p)x(t) + v(t))dt + Σ(k=2 a 5) Mk*Bᵢ(p)x(t)dwk, i = 1, ..., n,

onde Fⱼᵢ (i = 1, . . ., n; j = 1, ..., 5,) é o conjunto fuzzy de variáveis de estado, e denota o número da regra como n. Com base nas regras fuzzy acima, um mapeamento não linear, que pode aproximar o sistema não linear em (3), pode ser construído da seguinte forma:

dx(t) = [ Σ(i=1 a n)μᵢ(x) ((Aᵢ(p)x(t)+v(t))dt+Σ(k=2 a 5) Mk*Bᵢ(p)x(t)dwk) ] / [ Σ(k=1 a n)μk(x) ]
= Σ(i=1 a n)hᵢ(x)((Aᵢ(p)x(t) + v(t))dt + Σ(k=2 a 5) Mk*Bᵢ(p)x(t)dwk), (22)

onde μᵢ(x) = Π(j=1 a 5) Fⱼᵢ(xⱼ), hᵢ(x) = μᵢ(x) / Σ(k=1 a n)μk(x). As matrizes Aᵢ(p), Bᵢ(p), i = 1, 2, ..., n são especificadas de modo que Σ(i=1 a n)hᵢ(x)Aᵢ(p)x(t) e Σ(i=1 a n)hᵢ(x)Bᵢ(p)x(t) em (22) podem ser equivalentes a f(x, p) e g(x, t) em (3) pelo método de identificação fuzzy [16], respectivamente.
Então, o sistema considerado (9) pode ser aproximado por

dx̄(t) = Σ(i=1 a n)hᵢ(x̄) ( (Āᵢ(p)x̄(t)+v̄(t))dt + Σ(k=2 a 5) M̄k*B̄ᵢ(p)x̄(t)dwk ) (23)

onde x̄(t) = [x(t); x*(t)], Āᵢ(p) = [Aᵢ(p) 0; 0 Ar], M̄k = [Mk 0; 0 0], B̄ᵢ(p) = [Bᵢ(p), 0].

Seja V(x̄) = x̄ᵀPx̄ > 0 com V(0) = 0 uma função de Lyapunov para o sistema (23). Com base no método de aproximação e identificação fuzzy [16], temos

f̄(p, x̄, t) = Σ(i=1 a n)hᵢ(x̄)Āᵢ(p)x̄(t), ḡ(p, x̄, t) = Σ(i=1 a n)hᵢ(x̄)B̄ᵢ(p)x̄(t). (24)

Substituindo a fórmula acima nas HJIs em (12) e (18). Então, o problema de otimização (EPIP(γⱼ)) é equivalente ao seguinte Problema (FEPIP(γⱼ)):

(FEPIP(γⱼ)): min(p∈D) E(x̄ᵀ(0)Px̄(0))
s. t. P = Pᵀ > 0,
[ Āᵢᵀ(p)P + PĀᵢ(p) + Q + Σ(k=1 a 5) B̄ᵢᵀ(p)M̄kᵀPM̄k*B̄ᵢ(p)  P; P  -γⱼI ] ≤ 0,

[ Āᵢᵀ(p)P + PĀᵢ(p) + Q̄ + Σ(k=1 a 5) B̄ᵢᵀ(p)M̄kᵀPM̄k*B̄ᵢ(p)  P; P  -I ] ≤ 0.

Os Problemas de otimização acima (FEPIP(γⱼ)) são um modelo de otimização com restrições-LMI. Com o desenvolvimento da toolbox LMI baseada no método de ponto interior no MATLAB, a desigualdade matricial linear tem sido amplamente utilizada em sistemas e controle. Existem várias formas padrão do problema de desigualdade matricial linear, e o problema de otimização (FEPIP(γⱼ)) é um problema de autovalor (EVP). A análise teórica da eficiência desses algoritmos foi amplamente analisada nas Seções 3 e 4 no Capítulo 2 em Stephen et al. [26]. Aqui, damos os principais passos da seguinte forma:

**Algoritmo 1.**

**Passo 1 (Inicializar)** Defina um nível de ruído inicial γ, parâmetro α (0 < α < 1), especifique matrizes de perturbação Mk, k = 1, 2, 3, 4 e o vetor de parâmetros cinéticos inicial p ∈ D.
**Passo 2** Selecione funções de pertinência e regras da planta fuzzy para construir um modelo fuzzy T-S em (22) para aproximar o sistema estocástico não linear em (3), que fornece o sistema aumentado (23).
**Passo 3** Dado um nível de ruído γ, resolva o problema de otimização com restrições-LMI em (25) por algoritmo de busca da faixa admissível do vetor de parâmetros. Se houver a solução ótima, vá para o Passo 4. Caso contrário, pare e retorne a solução ótima.
**Passo 4** Se houver a solução ótima para o Passo 3, então faça γ = αγ e vá para o Passo 3.

**4. Resultados numéricos**

**4.1. Simulação numérica**

De fato, existem muitos microrganismos que podem fermentar glicerol em 1,3-PD, como *Klebsiella*, *Citrobacter* e *Clostridium*, etc. Nesta seção, consideramos um processo de fermentação em batelada de conversão de glicerol em 1,3-PD por *Klebsiella pneumoniae* (*K. pneumoniae*) sob condições anaeróbicas [27]. *K. pneumoniae* (DSM2026) usada neste estudo foi adquirida da Coleção Alemã de Microrganismos e Culturas Celulares (DSMZ) [28].

Na cultura de fermentação de glicerol, o meio de pré-cultura foi primeiramente inoculado em um biorreator de 5 L (BIOSTAT-B B.Braun Alemanha) com volume de trabalho de 4 L. A composição do meio aqui usado está listada na Tabela 1. A fermentação foi mantida estável a 37 °C. NaOH 40% (p/p) foi usado para ajustar o pH em 6.48-6.52. O tempo total de fermentação foi de 6.9 h. A taxa de alimentação de ar e rotação foram de 2 L/min e 300 rpm, respectivamente [29].

**Tabela 1**
Composição do meio de pré-cultura.
*(Tabela mostrando componentes químicos e suas concentrações)*

Para o mecanismo de fermentação, *K. pneumoniae* fermenta glicerol através das vias de oxidação e redução. Na via redutora, o glicerol é primeiramente convertido em 3-hidroxipropionaldeído (3-HPA) catalisado pela glicerol desidratase (GDHt), após o qual o 3-HPA é reduzido a 1,3-PD pela 1,3-propanodiol desidrogenase (PDDH). Neste processo, GDHt e PDDH desempenham um papel chave [30].

Durante a produção de 1,3-PD por *K. pneumoniae*, vários fatores (por exemplo, aeração e pH) foram estudados quanto a como afetam a regulação fina da via GDHt e PDDH, onde o pH influenciou significativamente a expressão genética de GDHt e PDDH, e resultou em flutuação dos produtos de fermentação [31]. Em [32], também foi demonstrado que a perturbação do pH na cultura tende à oscilação das taxas de formação e da taxa de consumo. Assim, a variância genética causada pela perturbação do pH pode ser caracterizada perturbando parâmetros matemáticos das taxas de formação e da taxa de consumo. Os parâmetros das taxas de formação e da taxa de consumo podem ser perturbados estocasticamente da seguinte forma:

mᵢ → mᵢ + Δmᵢnᵢ(t), Yᵢ → Yᵢ + ΔYᵢnᵢ(t), i = 2, 3, 4, 5, (26)

onde Δmᵢ e ΔYᵢ são os desvios padrão do parâmetro cinético, onde Δmᵢ = β × mᵢ e ΔYᵢ = β × Yᵢ, i = 2, 3, 4, 5. Aqui, β é chamado de parâmetro de controle de perturbação. Nesta subseção, seja β = 0.05. nᵢ(t) é um ruído branco Gaussiano com média zero e variância unitária, que denota a i-ésima fonte de flutuação aleatória.

No processo de fermentação biológica, existe uma inevitável ligeira variação da temperatura de fermentação e da concentração inicial de glicerol devido à tecnologia de medição. Para as diferentes concentrações de glicerol e temperaturas de cultura, os níveis de expressão gênica de GDHt e PDDH são similares na fermentação [33]. No entanto, fenômenos de oscilação das concentrações de produtos ainda podem ser observados em diferentes concentrações de glicerol e temperaturas de cultura [32]. Então, a variação das concentrações de glicerol e da temperatura de cultura pode ser vista como perturbações ambientais não hereditárias. Assim, a oscilação das concentrações de produtos causada por essas perturbações ambientais não hereditárias pode ser descrita por v̄ = (v₁, v₂, v₃, v₄, v₅)ᵀ ∈ L²F([0, tf], ℝ⁵), e neste artigo, supomos que vᵢ(t), i = 1, 2, 3, 4, 5 sejam uniformemente distribuídos em [-θ, θ], onde θ também é um parâmetro de controle de perturbação. Nesta subseção, fazemos θ = 0.025. Através da análise acima, sabemos que perturbações ambientais externas não hereditárias e perturbações intrínsecas hereditárias podem ser descritas pelo vetor de parâmetros de controle de perturbação (θ, β).

Nesta seção, o sistema estocástico não linear (3) é primeiramente aproximado a uma função linear por partes empregando o sistema fuzzy T-S. Aqui, fazemos o número de regras fuzzy ser n = 30, e as funções de pertinência do conjunto fuzzy Fⱼᵢ serem funções do tipo triangular. Então, o modelo fuzzy T-S pode ser dado da seguinte forma [16]:

*(Regra Fuzzy i é apresentada aqui)*

onde Aᵢ(p) = [l(p) 0], Bᵢᵏ(p) = [βhᵏ(p) 0], 0 = [0]₅ₓ₄, e h²(p) = (0, −m₂ + aᵢY₂, 0, 0, 0)ᵀ, h³(p) = (0, 0, m₃ + aᵢY₃, 0, 0)ᵀ, h⁴(p) = (0, 0, 0, m₄ + aᵢY₄, 0)ᵀ, h⁵(p) = (0, 0, 0, 0, m₅ + aᵢY₅)ᵀ. l(p) = (aᵢ, −m₂ + aᵢY₂, m₃ + aᵢY₃, m₄ + aᵢY₄, m₅ + aᵢY₅)ᵀ. Aqui, aᵢ(i = 1, ..., 30) são parâmetros a serem identificados.

Neste trabalho, estimaremos parâmetros cinéticos desconhecidos em (3) de modo a determinar o modelo do sistema biológico com base nos dados experimentais. O Problema aproximado {(FEPIP(γⱼ))}ⱼ≥₁ foi então resolvido pelo Algoritmo 1. Neste artigo, escrevemos um programa Matlab 7.10.0 para implementar o Algoritmo 1, onde a toolbox LMI no Matlab é usada para resolver os problemas de otimização com restrições-LMI.

Pelo Algoritmo 1, obtivemos os parâmetros cinéticos ótimos p* = (0.0466, 0.0049, -12.0095, 195.509, 3.7281, 19.7334, -1.9085, 29.0468)ᵀ. A Fig. 1 mostra a comparação de dados experimentais e resultados computacionais, onde as linhas verdes e outras linhas coloridas representam resultados computacionais pelo modelo fuzzy T-S e pelo sistema dinâmico estocástico não linear, respectivamente. Além disso, usamos outros dados experimentais como dados de teste para verificar a confiabilidade do modelo, onde a biomassa inicial e a concentração de glicerol são 0.102 g/L e 418.26 mmol/L, respectivamente. No novo experimento, o tempo total de fermentação foi de 6.6 h. Os resultados da simulação também são dados na Fig. 2. Das Figs. 1 e 2, podemos ver que os resultados da simulação são anastomóticos com o experimento.

*(Fig. 1. Comparação de resultados estimulados e experimentais de biomassa, glicerol, 1,3-PD, acetato e etanol na cultura em batelada com biomassa inicial e concentração de glicerol de 0.173 g/L e 402.935 mmol/L.)*

*(Fig. 2. Comparação de resultados estimulados e experimentais de biomassa, glycerol, 1,3-PD, acetato e etanol na cultura em batelada com biomassa inicial e concentração de glicerol de 0.102 g/L e 418.261 mmol/L.)*

Defina o erro relativo das variáveis de estado como

ek% = (1/K) Σ(i=1 a K) |xk(ti) – xk*(ti)| / xk*(ti), k = 1, 2, 3, 4, 5,

onde xk(ti) é o valor calculado pelo sistema estocástico (3) no tempo ti, xk*(ti) é o dado de teste experimental no tempo ti, e K é o número de testes realizados em um experimento. Realizando 400 simulações numéricas, os erros relativos e% = (e₁%, e₂%, e₃%, e₄%, e₅%) = (0.3254, 0.1643, 0.1261, 0.2618, 0.1335) podem ser obtidos para as cinco substâncias desta fermentação microbiana. Os erros relativos médios das cinco substâncias são ē% = (1/5) Σ(k=1 a 5) ek% = 0.2022. Portanto, com base na análise acima, temos razões para acreditar que o sistema proposto (3) com os parâmetros ótimos atende aos requisitos de rastreamento de dados experimentais. Aqui, o erro relativo da biomassa é significativamente maior que o das outras substâncias. Há uma razão possível que a constante de saturação ks seja predeterminada incorretamente como 0.28 de Xiu et al. [17]. A discussão da constante de saturação de Monod ks ultrapassou o escopo deste artigo. Os valores dos parâmetros do sistema fuzzy identificado também são dados na Tabela 2. Para mostrar que o sistema fuzzy pode aproximar o sistema original, resultados simulados com θ = 0, β = 0 são mostrados na Fig. 3.

**Tabela 2**
Os valores dos parâmetros do sistema fuzzy identificado.
*(Tabela mostrando os parâmetros a1 a a30)*

*(Fig. 3. Comparação de resultados estimulados pelo modelo fuzzy T-S (22) e sistema dinâmico estocástico não linear (3) com (θ = 0, β = 0).)*

Finalmente, realizamos 100 simulações estocásticas do sistema (3) e desenhamos separadamente as trajetórias correspondentes das concentrações em questão com os parâmetros ótimos, e os resultados são mostrados na Fig. 4. Intuitivamente, as variáveis de estado são menos sensíveis à perturbação ambiental. Portanto, é uma conclusão aceitável que o sistema proposto (3) com os parâmetros ótimos atende aos requisitos de robustez.

*(Fig. 4. As variações nas trajetórias de biomassa, glicerol, 1,3-PD, acetato e etanol realizando 100 simulações.)*

**4.2. Análise de perturbação ambiental**

Com base na análise acima na subseção de Simulação Numérica, podemos saber que o sistema estocástico proposto (3) pode descrever o processo de fermentação em batelada sob perturbações ambientais. Aqui, as perturbações ambientais podem ser descritas pelo vetor de parâmetros de perturbação. Nesta subseção, queríamos explorar como as perturbações ambientais afetam o processo de fermentação microbiana pela análise de simulação do modelo matemático (3). Realizando 400 simulações numéricas, o erro relativo médio pode ser obtido e listado na Tabela 3. Da Tabela 3, algumas informações significativas podem ser obtidas. Se o ambiente externo é bem controlado (ou seja, θ = 0), é razoável acreditar que existem perturbações ambientais hereditárias (β = 0.03 ou β = 0.04) no processo de experimento de fermentação microbiana. Similarmente, se β = 0, então, existe perturbação ambiental externa (θ = 0.03) para este experimento de fermentação. A Tabela 3 mostra que o vetor de parâmetros de perturbação mais apropriado pode ser (θ*, β*) = (0.03, 0.03) para o ambiente experimental atual. No entanto, da Tabela 3, também podemos ver que o erro relativo é 0.2508 quando (θ, β) = (0, 0). Portanto, é uma inferência razoável que exista perturbação ambiental neste processo de fermentação microbiana. Para comparação, os resultados da simulação de 1,3-PD e Etanol com diferentes valores de parâmetros de perturbação são mostrados na Fig. 5.

**Tabela 3**
Comparação do erro relativo médio sob diferentes parâmetros.
*(Tabela mostrando e% para diferentes combinações de θ e β)*

*(Fig. 5. Resultados da simulação de 1,3-PD, etanol sob (θ = 0.05, β = 0.3), (θ = 0.5, β = 0.03) e (θ = 0.03, β = 0.03).)*

**5. Conclusões e discussões**

Neste artigo, com base no mecanismo de fermentação microbiana e nas características das perturbações ambientais no sistema de fermentação microbiana, um sistema estocástico não linear é construído para descrever o processo de fermentação em batelada de glicerol. Para determinar o modelo matemático, os parâmetros cinéticos ótimos e os parâmetros de perturbação são obtidos com base nos dados experimentais e nas características básicas da robustez biológica. E, da Tabela 3, podemos ver que o erro relativo médio mínimo é e% = 0.1937, e a perturbação do ambiente externo é uniformemente distribuída em [-0.03, 0.03] e a perturbação ambiental interna é perturbação paramétrica de β = 0.03. No entanto, da Tabela 3, também podemos ver que o erro relativo médio é 0.2508 quando (θ, β) = (0, 0). Ou seja, o modelo matemático com parâmetros de perturbação é mais consistente com os dados experimentais do que o modelo sem perturbação para este processo de fermentação microbiana. Deve-se notar que quando θ = 0 e (θ, β) = (0, 0), o modelo proposto degenera para o modelo em Wang et al. [6] e Gao et al. [34], respectivamente. Além disso, o erro relativo médio ē% = 0.1937 neste artigo é menor que o erro relativo ē% = 0.2613 em Gao et al. [34].

De fato, há muitas perturbações nos sistemas de fermentação microbiana que são difíceis de serem superadas no processo experimental. Essas perturbações às vezes interferem seriamente nos resultados experimentais. No entanto, não é realista realizar muitos experimentos para analisar o impacto das perturbações ambientais no rendimento devido ao alto custo do experimento. É bem sabido que a modelagem matemática é uma ferramenta importante para a análise teórica. Portanto, é um passo chave formular o processo de fermentação por um modelo matemático preciso. Assim, acreditamos que o resultado deste trabalho pode fornecer uma referência para a prática industrial real.

Neste artigo, a simulação da concentração de biomassa não se ajusta bem o suficiente em comparação com os resultados experimentais. Achamos que a causa pode ser que a constante de saturação ks seja alterada devido à perturbação ambiental, o que será investigado como uma continuação deste trabalho. Embora os parâmetros cinéticos e os parâmetros de perturbação no sistema proposto possam ser determinados com sucesso pelo nosso algoritmo e avaliação de simulação aproximada. Mas leva 26 h para realizar totalmente este cálculo, o que é caro em termos de custo. Em nosso estudo futuro, exploraremos novos métodos para resolver efetivamente tais problemas.

**Agradecimentos**

Este trabalho foi apoiado pela Fundação Nacional de Ciências Naturais da China (Grant no. 11771008), pela Fundação de Ciências Naturais da Província de Shandong, China (Grant no. ZR2015FM014), pela Fundação de Ciência Pós-Doutoral da China (Grant no. 2015M572061) e pela Fundação de Ciência Pós-Doutoral de Qingdao, China.

**Referências**

*(A lista de referências é mantida como no original)*

---