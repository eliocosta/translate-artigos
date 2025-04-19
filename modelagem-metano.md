Okay, here is the translation of the scientific article into Brazilian Portuguese, maintaining the original information and structure.

---

**Renewable Energy 211 (2023) 296-306**

**Conteúdo disponível em ScienceDirect**

**Renewable Energy**

**página inicial da revista: www.elsevier.com/locate/renene**

**Uso de resultados do potencial metanogênico bioquímico para a otimização econômica de sistemas contínuos de digestão anaeróbia: o efeito da sinergia dos substratos**

**Georgios Manthos, Margarita Dareioti, Dimitris Zagklis, Michael Kornaros***

Laboratório de Engenharia Bioquímica e Tecnologia Ambiental (LBEET), Departamento de Engenharia Química, Universidade de Patras, Rua Karatheodori 1, Campus Universitário, 26504, Patras, Grécia

**INFORMAÇÕES DO ARTIGO**

*Palavras-chave:*
Co-digestão
Modelagem
Avaliação técnico-econômica
Tomada de decisão
Potencial metanogênico bioquímico
Digestão anaeróbia

**RESUMO**

Durante o processamento de matérias-primas agrícolas do setor primário, grandes quantidades de subprodutos com alto conteúdo de energia química são produzidos. Alguns destes são as águas residuárias de lagares de azeite (OMW), soro de leite (CW) e esterco líquido bovino (LCM). A digestão anaeróbia é um processo promissor e ambientalmente amigável para a valorização energética de subprodutos agroindustriais e pecuários. O objetivo deste estudo foi a modelagem matemática da digestão anaeróbia em sistemas em batelada, visando quantificar possíveis sinergias que ocorrem entre substratos complementares. A análise baseou-se no uso de dados de potencial metanogênico bioquímico para prever o tempo ótimo de retenção hidráulica (HRT) sob condições de estado estacionário de sistemas contínuos, para diferentes razões de substrato. A função objetivo para a otimização do HRT baseou-se na maximização do lucro do processo e incluiu parâmetros técnico-econômicos, permitindo a comparação das diferentes razões de substrato que podem ser usadas na alimentação. A co-digestão com uma razão de mistura OMW:LCM igual a 70:30 provou-se muito satisfatória para a sustentabilidade do processo, exibindo um lucro líquido máximo de 16 €/m³reator/d para uma capacidade de planta de 10 m³alimentação/d.

**1. Introdução**

Subprodutos agroindustriais são uma importante questão ambiental e social em todo o mundo, já que aproximadamente 1 bilhão de toneladas desses materiais são gerados globalmente a cada ano. Especificamente na Grécia, certas agroindústrias, como lagares de azeite e fazendas leiteiras, e plantas de processamento representam uma parcela considerável do problema ambiental nos países mediterrâneos, produzindo grandes quantidades de efluentes líquidos como águas residuárias de lagares de azeite (OMW), soro de leite (CW) e esterco bovino. Apesar dos benefícios econômicos da produção desses materiais agroindustriais, os países produtores devem lidar com várias questões ambientais. Em muitos casos, essas correntes são descartadas diretamente em aterros sanitários ou corpos d'água inadequados [1].

A filosofia de desperdício zero é um sistema de gerenciamento de resíduos e uma solução para os problemas que os resíduos criam. Sua implementação promove o desenvolvimento sustentável e a recuperação de recursos, reduz a disposição de resíduos em aterros sanitários ou corpos d'água, e inclui a prevenção da geração de resíduos e o design adequado do produto considerando todo o seu ciclo de vida [2].

A conversão de biomassa em energia é tipicamente realizada usando dois grupos principais de processos: termoquímicos e biológicos [3]. Na maioria dos casos, os processos termoquímicos são mais economicamente viáveis, mas mais custosos ambientalmente do que os processos biológicos [4,5]. A digestão anaeróbia é um processo biológico que está em linha com os princípios mencionados acima, uma vez que o principal produto do processo (biometano) pode substituir parcialmente os combustíveis fósseis [6]. Além disso, a digestão anaeróbia é um método eficiente de tratamento de resíduos, pois pode funcionar com altas taxas de carregamento orgânico com ótimo desempenho de degradação [7,8]. Em relação aos benefícios ambientais, a substituição de combustíveis fósseis por biocombustíveis pode reduzir as emissões globais de gases de efeito estufa.

Uma forma eficiente de tratamento de resíduos via digestão anaeróbia é a co-digestão de diferentes substratos. Muitos pesquisadores apresentam resultados promissores para a co-digestão anaeróbia de diferentes tipos de resíduos com alta complementaridade, como resíduo de batata e esterco suíno [9], fraldas descartáveis usadas e produtos alimentícios vencidos [10], resíduos alimentares e borra de café [11]. A seleção de diferentes correntes de resíduos é um parâmetro crítico para a eficiência do processo, pois pode levar a um aumento na produtividade de metano.

A descrição matemática dos efeitos sinérgicos de diferentes razões de mistura de substratos pode ser uma ferramenta útil para selecionar as correntes de substrato apropriadas, levando em conta a capacidade da planta de tratamento e seu custo operacional total [12]. Muitos modelos matemáticos diferentes têm sido usados para descrever tais processos, incluindo o Modelo de Digestão Anaeróbia No. 1 (ADM1) e equações algébricas sigmoidais. A equação de Gompertz modificada é um modelo algébrico sigmoidal adequado para uso generalizado devido à sua simplicidade e ao significado físico de seus parâmetros [13].

A construção de uma planta de digestão anaeróbia para produção de energia é considerada um investimento de alto risco por muitas empresas e investidores [14]. Para superar essa questão, muitos governos estabeleceram leis de desenvolvimento para subsidiar unidades de digestão anaeróbia, visando apoiar as indústrias 'verdes' e a energia renovável [15]. O custo de capital dessas unidades depende fortemente do equipamento e das características qualitativas e quantitativas da alimentação. Correntes de resíduos com baixas taxas de produção de metano podem levar a grandes volumes de reator e altos custos de capital [16].

O objetivo deste trabalho foi o estudo matemático dos efeitos sinérgicos na co-digestão de diferentes subprodutos agroindustriais em testes de Potencial Metanogênico Bioquímico (BMP) para uso na tomada de decisão durante o projeto de sistemas contínuos em escala real. Três substratos diferentes foram usados, nomeadamente águas residuárias de lagares de azeite (OMW), soro de leite (CW) e esterco líquido bovino (LCM), em diferentes razões de mistura ou como substratos puros. Subsequentemente, a modelagem matemática dos testes de BMP usando a equação de Gompertz modificada, com a adição de termos extras para descrever os efeitos sinérgicos, foi realizada. Finalmente, os resultados desta análise foram usados para projetar uma planta otimizada considerando parâmetros técnicos e econômicos visando a maximização da sustentabilidade econômica. Esta análise pode ser usada como uma ferramenta simples para o projeto da planta de processos contínuos em escala real e tomada de decisão para as condições ótimas de operação de uma planta de digestão anaeróbia.

---

**Abreviações**

*   **ADM1** Modelo de Digestão Anaeróbia 1
*   **BMP** Potencial Metanogênico Bioquímico
*   **CHP** Unidade de Cogeração de Calor e Energia
*   **COD** Demanda Química de Oxigênio
*   **CW** Soro de Leite
*   **HRT** Tempo de Retenção Hidráulica
*   **LCM** Esterco Líquido Bovino
*   **OMW** Águas Residuárias de Lagares de Azeite
*   **TS** Sólidos Totais
*   **VS** Sólidos Voláteis
*   **S** Concentração de substrato dentro do reator
*   **S0** Concentração de substrato no material de alimentação
*   **SnBMP** Parâmetro de sinergia para BMP
*   **Snlag** Parâmetro de sinergia para lag
*   **SnRm** Parâmetro de sinergia para Rm
*   **Vr** Volume do reator
*   **VSadded** SV de substrato adicionado em cada reator
*   **VSfeed** SV do material de alimentação
*   **VSsludge** SV do inóculo
*   **x** Concentração de biomassa
*   **Yexp** Dados experimentais
*   **Ysim** Dados estimados numericamente
*   **Yx/S** Coeficiente de rendimento para biomassa do substrato
*   **Δh** Diferença de altura manométrica multiplicada pela aceleração da gravidade
*   **λ** Razão Substrato/lodo

**Nomenclatura**

*   **Ks** Constante de Monod
*   **lag** A fase lag dos microrganismos
*   **Q** Vazão volumétrica
*   **Rm** Taxa máxima de produção de metano

---

**2. Materiais e métodos**

**2.1. Material de alimentação e inóculo**

Diferentes materiais de certas agroindústrias foram usados como alimentação dos reatores anaeróbios durante os testes iniciais de BMP. OMW, CW e LCM foram obtidos de indústrias locais na região da Acaia, Grécia. Os materiais de alimentação foram armazenados separadamente a -18 °C até o uso. As características físico-químicas das matérias-primas são apresentadas na Tabela 1. O resultado da caracterização dos substratos brutos mostrou que OMW, CW e LCM tinham características diferentes. A quantidade e a qualidade da matéria orgânica foram muito diferentes entre os substratos, assim como seu conteúdo de nutrientes, como nitrogênio e fósforo.

O lodo anaeróbio que foi usado no procedimento experimental foi obtido de uma estação de tratamento de efluentes em Metamorphosis (Ática, Grécia). O teor de sólidos voláteis do lodo era de 1,13 g/L.

**Tabela 1**
Características físico-químicas dos substratos brutos.

| Parâmetro                      | OMW             | CW              | LCM             |
| :----------------------------- | :-------------- | :-------------- | :-------------- |
| pH                             | 5.36 ± 0.16     | 6.32 ± 0.36     | 8.82 ± 0.22     |
| TS [g/L]                       | 73.50 ± 1.01    | 64.40 ± 0.39    | 20.30 ± 0.36    |
| VS [g/L]                       | 55.97 ± 0.36    | 55.72 ± 0.32    | 12.47 ± 0.22    |
| COD Total [g/L]                | 85.23 ± 3.21    | 77.26 ± 0.15    | 21.37 ± 0.72    |
| Carboidratos Totais [g/L]      | 34.70 ± 1.09    | 41.00 ± 1.03    | 2.13 ± 0.08     |
| Fenóis totaisª [g/L]           | 7.71 ± 0.70     | N.D.            | N.D.            |
| Nitrogênio total [g/L]         | 0.42 ± 0.02     | 0.95 ± 0.03     | 2.52 ± 0.07     |
| Gorduras e Óleos [g/L]         | 9.06 ± 0.93     | 0.66 ± 0.01     | 0.71 ± 0.25     |
| Carbono [%]                    | 53.45 ± 1.18    | 41.94 ± 0.92    | 41.55 ± 0.27    |
| Hidrogênio [%]                 | 6.65 ± 0.02     | 5.15 ± 0.51     | 5.37 ± 0.16     |
| Nitrogênio [%]                 | 0.90 ± 0.07     | 1.36 ± 0.10     | 1.90 ± 0.17     |
| Cinzas [%]                     | 23.85 ± 0.44    | 13.48 ± 0.81    | 38.57 ± 0.40    |
| Oxigênio [%]                   | 15.15 ± 0.74    | 38.07 ± 0.98    | 12.61 ± 0.66    |

ª Em equivalentes de ácido siríngico.

**2.2. Técnicas analíticas**

O pH da amostra foi determinado por um medidor de pH com um eletrodo (Thermo Scientific, Orion ROSS Ultra Refillable pH/ATC Triode). O teor de Sólidos Totais (TS) foi calculado pesando uma quantidade de amostra fresca antes e após a secagem a 105 °C de acordo com os Standard Methods [17]. O teor de Sólidos Voláteis (VS) foi determinado medindo o peso da amostra seca antes e após a queima a 550 °C. A Demanda Química de Oxigênio (COD) Total e os carboidratos totais foram estimados fotometricamente de acordo com os Standard Methods [17] e Joseffson [18], respectivamente. Os compostos fenólicos totais foram determinados usando o reagente de Folin-Ciocalteu e expressos em equivalentes de ácido siríngico [19,20]. O Nitrogênio total foi medido convertendo o nitrogênio total em amônia livre e quantificado com um aparelho de Kjeldahl [17], enquanto gorduras e óleos foram determinados após extração com hexano usando um aparelho Soxhlet (Velp Scientifica, SER 148). A análise elementar foi realizada após liofilização das amostras brutas (Telstar, LyoQuest apparatus). A caracterização elementar foi feita usando um analisador elementar (EA3000, Eurovector) de acordo com Tsigkou et al. [7].

A composição do biogás (metano e dióxido de carbono) foi analisada por cromatografia gasosa (Agilent Technologies 7890 A) equipada com uma coluna capilar (HP-PLOT/Q, 30 m de comprimento, 0,53 mm D.I. e 40 µm de filme de empacotamento) e um detector de condutividade térmica (TCD) usando nitrogênio como gás de arraste. A temperatura do injetor e do detector foi mantida a 250 °C, e a temperatura do forno foi gradualmente aumentada de 80 °C (mantida por 6 min) para 200 °C (mantida por 2 min) a uma taxa de 50 °C/min.

**2.3. Montagem experimental e procedimento**

A principal montagem experimental é apresentada na Fig. 1. Cada substrato foi analisado em duplicata, enquanto dois frascos adicionais contendo apenas inóculo foram incluídos para contabilizar a produção de metano de fundo (endógena) (branco). Resumidamente, quantidades conhecidas de substrato (0,16 ± 0,04 g VS por frasco) e inóculo anaeróbio ativo (20% v/v) foram adicionados a frascos de soro de 160 mL. A razão final VSinóculo/VSsubstrato foi estabelecida em 4 de acordo com [21]. Meio definido adicional contendo nutrientes e vitaminas para culturas anaeróbias mistas também foi adicionado e o pH foi medido, de acordo com [22]. Os frascos de soro foram purgados por 5 min com gás nitrogênio e então selados imediatamente usando septos de borracha butílica e lacres de alumínio. Uma vez selados, os frascos foram colocados em um banho-maria com agitação orbital (Grant OLS200) a 80 rpm e mantidos a uma temperatura mesofílica constante (37 °C). A medição do gás produzido foi realizada usando uma seringa plástica para quantificar a sobrepressão dentro do frasco de soro. A qualidade do biogás produzido foi determinada usando Cromatografia Gasosa (Agilent Technologies 7890 A) equipada com uma coluna capilar (HP-PLOT/Q, 30 m de comprimento, 0,53 mm D.I. e 40 µm de filme de empacotamento). O método seguido neste trabalho baseou-se em um procedimento experimental simples e equações matemáticas básicas para facilitar o uso e a aplicabilidade mais ampla. Quinze misturas de substratos foram preparadas para examinar potenciais efeitos sinérgicos durante a co-digestão de substratos. Mais especificamente, os três substratos foram co-digeridos em pares sob diferentes razões de substrato (SOMW: SLCM, SCW: SLCM, SOMW: Scw) variando de 0% a 100% v/v com um passo de 25%. Além disso, a co-digestão de todos os três substratos foi realizada sob três diferentes razões de mistura de SOMW: SCW: SLCM (50:25:25, 25:50:25 e 25:25:50). O escopo desta metodologia foi avaliar uma ampla área de diferentes razões de substrato visando fornecer um conjunto de dados válido para calibração do modelo.

*(Fig. 1. Montagem experimental para testes de BMP. Inclui imagens de frascos OMW, CW, LCM, um frasco de soro selado com medição de gás.)*

**2.4. Desenvolvimento do modelo**

A estrutura do modelo proposta foi baseada na equação de Gompertz modificada (Equação (1)):

Metano(t) = BMP exp(-exp( (Rm * e / BMP) * (lag - t) + 1 )) --- **Equação 1**

Onde BMP corresponde ao rendimento máximo de metano do reator (Lmetano/g VSadicionado), Rm indica a taxa máxima de produção de metano nessas condições (Lmetano/g VSadicionado/d) e lag é representativo do período de ajuste dos microrganismos nas condições do reator (d). Esta equação foi usada para alcançar uma análise simples e fácil de usar. Nesta direção, a análise proposta poderia dar uma perspectiva geral do processo bioquímico considerando tanto a produção acumulada de metano quanto a taxa máxima de produção de metano. Todos os efeitos inibitórios são agrupados nos diferentes valores dos parâmetros de Gompertz (BMP, Rm, lag) para cada cenário de substrato. Um modelo mais complexo, como o ADM1, poderia ser potencialmente usado para alcançar maior precisão, mas com maior complexidade.

Diferentes conjuntos dos três parâmetros de Gompertz foram calculados para cada matéria-prima testada (OMW, CW e LCM) usando uma função objetivo (Equação (2)), onde yexp,i.j representa os dados experimentais e ysim,i,j os dados estimados numericamente. Além disso, o contador i denota o número de dados experimentais de cada teste (variável), enquanto o contador j denota o número de diferentes substratos. A etapa de estimação dos parâmetros de Gompertz e a estimação do intervalo de confiança foram realizadas usando o software MATLAB e o suplemento Solver do Microsoft Excel. A metodologia do intervalo de confiança é descrita no trabalho de Tsafrakidou et al. [23].

min Σ(j=1 a m) Σ(i=1 a n) (yexp,i,j – ysim,i,j)² --- **Equação 2**

Os parâmetros da equação de Gompertz de potencial metanogênico máximo, taxa máxima de produção de metano e fase lag para o substrato bruto foram mantidos constantes para o treinamento do modelo ao usar os dados de co-digestão. Um elemento chave da análise foi a quantificação do efeito de sinergia exibido durante a co-digestão. Por esta razão, parâmetros extras foram incluídos na equação final do modelo para indicar o efeito de sinergia em cada parâmetro da equação de Gompertz modificada. As razões de mistura volumétricas foram convertidas para razões de VS para a implementação dos conjuntos de dados de mistura. A fração de sólidos voláteis para cada matéria-prima em cada biorreator diferente foi representada com o parâmetro wi.

Em relação à quantificação da sinergia do substrato, considerou-se necessário implementar este efeito em todos os três parâmetros da equação de Gompertz (BMP, Rm e lag), a fim de descrever a influência de diferentes razões de substrato no processo biológico. Muitos autores relataram que as diferentes razões de mistura têm uma influência significativa no rendimento máximo de metano, bem como na taxa de produção de metano dos consórcios microbianos [24,25]. Os termos de sinergia na equação final do modelo foram representados com os termos SnBMP, SnRm e Snlag (Equação (3)).

Metano(wi, t) = SnBMP Σ(i=OMW,CW,LCM) (wi * BMPi) * exp(-exp( (SnRm * Σ(i=OMW,CW,LCM) (wi * Rm,i) * e) / (SnBMP * Σ(i=OMW,CW,LCM) (wi * BMPi)) * (Snlag * Σ(i=OMW,CW,LCM) (wi * lagi) - t) + 1 )) --- **Equação 3**

Diferentes parâmetros de sinergia foram estimados para cada mistura para mapear o efeito nos pontos de mistura. Equações matemáticas polinomiais empíricas foram usadas para converter os valores quantizados para cada mistura experimental em funções contínuas. Essas equações podem não ter um significado físico fortemente definido, mas foram avaliadas como uma ferramenta útil para a análise. Esta etapa foi feita usando o Software Minitab 18.

**2.5. Projeto da planta de reatores contínuos e avaliação técnico-econômica**

O modelo matemático desenvolvido pode ser potencialmente usado para simular o processo biológico em uma planta de escala real, fornecendo previsões do desempenho da planta sob diferentes condições. No nosso caso, o modelo desenvolvido foi usado para projetar uma planta simplificada de digestão anaeróbia que pudesse processar 10 m³ de alimentação por dia. A variável de otimização foi a razão de mistura do substrato, e o alvo da otimização foi maximizar o lucro da planta em euros por m³ de reator por dia. O projeto de um processo ótimo de digestão anaeróbia de um substrato específico é sensível a múltiplos fatores, considerando a complexidade do sistema. Portanto, a análise proposta constitui uma simulação em condições de estado estacionário, não levando em conta o período crítico de partida do reator, onde a aclimatação da biomassa precisa ser considerada. Certos experimentos em sistemas contínuos em escala de laboratório e piloto poderiam ser realizados para testar a validade do método proposto.

O equipamento da planta incluía um tanque de alimentação, duas bombas para alimentação e efluente, um reator de parede dupla com isolamento e agitação, e uma unidade de CHP (Cogeração de Calor e Energia) para produção de energia térmica e elétrica (Fig. 2). O tempo ótimo de retenção hidráulica (HRT) do processo é um parâmetro importante, pois afeta o tamanho e os requisitos energéticos do reator.

*(Fig. 2. Equipamento da planta considerado para o processo contínuo de digestão anaeróbia. Inclui Tanque de alimentação, Reator, Bombas e Unidade CHP.)*

Várias suposições e limitações podem reduzir a precisão do modelo proposto, especialmente ao estimar o desempenho de um sistema contínuo em escala real a partir de experimentos em batelada em escala laboratorial. Por outro lado, a análise proposta é simples e equipamento mínimo é necessário para sua implementação.

As suposições feitas para a análise foram que o parâmetro Rm da equação de Gompertz era a taxa intrínseca dos microrganismos e que o sistema contínuo em escala real operaria em condições de estado estacionário. Além disso, assumiu-se que apenas uma porção do COD total do substrato era biodegradável. A parte biodegradável do COD foi estimada através do parâmetro BMP da equação de Gompertz para cada mistura de acordo com a Equação (4).

S0 [g COD/L] = (BMP [NL/g VS] / 0.35 [NL/g COD]) * VSfeed [g VS/L] --- **Equação 4**

Onde VSfeed representa o VS do material de alimentação para cada cenário de mistura em g/L. O valor 0,35 representa a conversão estequiométrica de 1 g de COD para 0,35 L de metano.

Os balanços de massa do substrato e da biomassa microbiana foram usados na análise. A cinética de Monod foi usada para descrever a limitação da taxa máxima pela depleção do substrato. Os balanços de massa são apresentados nas Equações (5), (6).

dS/dt [g COD/L/d] = (S0 [g COD/L] / HRT [d]) - (S [g COD/L] / HRT [d]) - (Rm [NL/g COD/d] / 0.35 [NL/g COD]) * (S [g COD/L] / (S [g COD/L] + Ks [g COD/L])) * [gsub/gsl] * x [g COD/L] --- **Equação 5**

dx/dt [g COD/L/d] = - (x [g COD/L] / HRT [d]) + Yx/s * (Rm [NL/g COD/d] / 0.35 [NL/g COD]) * (S [g COD/L] / (S [g COD/L] + Ks [g COD/L])) * [gsub/gsl] * x [g COD/L] --- **Equação 6**

Onde S representa a concentração de substrato dentro do reator [g COD/L], x representa a concentração de biomassa dentro do reator (concentração negligível de biomassa foi considerada na alimentação) [g COD/L], S0 representa a concentração inicial de substrato na alimentação [g COD/L], Ks apresenta a constante de Monod, Yx/s o coeficiente de rendimento para biomassa do substrato e λ indica a razão substrato/lodo em termos de VS. Os valores para os parâmetros Ks e Yx/s foram 0,3 g COD/L e 0,1 g COD,lodo/g COD,substrato, respectivamente [26]. O parâmetro λ foi calculado a partir da Equação (7):

λ = VSadded [g VS] / (VSi [g/L] * Vr [L] * 0.2 [L/L]) --- **Equação 7**

Onde VSi representa o VS do inóculo em g/L (VSi = 1,13 g/L) e Vr representa o volume do reator (Vr = 0,16 L). O termo constante 0,2 indica os 20% v/v de inóculo nos sistemas BMP. É importante notar que os termos de Rm e BMP difeririam para o cenário de mistura e seriam estimados através das equações empíricas do procedimento de modelagem matemática.

A partir das condições de estado estacionário, os termos de acumulação foram definidos como zero:

0 = (S0 / HRT) - (S / HRT) - (Rm / 0.35) * (S / (S + Ks)) * λx --- **Equação 8**

0 = - (x / HRT) + Yx/s * (Rm / 0.35) * (S / (S + Ks)) * λx --- **Equação 9**

A concentração de biomassa em estado estacionário pode ser estimada (Equação (10)):

x = Yx/s * (S0 - S) --- **Equação 10**

A equação final para a estimação da concentração de substrato no efluente foi calculada após substituição:

S² * (- (1/HRT) * (1 / (λ * Yx/s))) + S * ( (S0/HRT) * (1 / (λ * Yx/s)) - (Ks / (λ * Yx/s)) + (Rm / (0.35 * λ)) ) + (S0 * Ks / (HRT * λ * Yx/s)) = 0 --- **Equação 11**

Finalmente, a produtividade total do reator contínuo foi estimada a partir da diferença entre a matéria orgânica de entrada e saída de acordo com a Equação (12).

Produtividade [m³ CH4 / m³ alimentação] = 0.35 * (S0 - S) --- **Equação 12**

Considerando os aspectos técnicos e econômicos do processo, um projeto detalhado do equipamento foi realizado. A estimação do custo de capital do reator foi feita considerando que o tanque do reator era de parede dupla com uma camada de isolamento. Para o custo da parede dupla do reator, assumiu-se que ele pode consistir em dois tanques de aço inoxidável 316. O tanque externo foi considerado com um raio 20% maior que o tanque interno. O custo dos tanques foi calculado de acordo com a Equação (13) [27]:

Cptanque($@1979) = exp{9.369 – 0.1045(lnV) + 0.045355(lnV)²} --- **Equação 13**

onde V representa o volume do reator que foi calculado a partir do HRT do processo. O custo foi normalizado usando os indicadores Marshall & Swift para 2020. O isolamento consistia em poliuretano. Os tanques de alimentação e efluente foram projetados para ter a capacidade de armazenar a alimentação e o efluente de dois dias de operação do biorreator.

O custo das bombas foi estimado a partir da Equação (14) & Equação (15) [27]:

S = Q * √Δh --- **Equação 14**

Custo da bomba($@1979) = exp [7.2234 + 0.3451 ln(S) + 0.0519ln(S)²] --- **Equação 15**

onde Q representa a vazão volumétrica requerida e Δh é a diferença de altura manométrica multiplicada pela constante de aceleração gravitacional (g). O custo foi normalizado usando os indicadores Marshall & Swift para 2020.

Finalmente, para a purificação e utilização do biogás produzido, um sistema foi projetado que incluía uma torre de dessulfurização, bem como uma unidade de cogeração para energia elétrica e térmica se a produtividade da unidade fosse maior que 65 kW. A equação usada foi calculada de acordo com a Equação (16) [28]:

Custo CHP (€) = 1257.02 x Capacidade [kWe] --- **Equação 16**

Onde o termo Capacidade representa os kW de eletricidade produzidos pela unidade.

Os requisitos de energia térmica e elétrica do sistema foram calculados considerando a temperatura externa e interna do reator (17 °C e 37 °C respectivamente) e as demandas elétricas do agitador e da bomba.

O custo operacional da unidade foi estimado levando em conta o custo da energia elétrica, bem como a depreciação do equipamento, uma vez que a vida útil do equipamento foi definida em 10 anos, de acordo com a Equação (17). Os requisitos de energia térmica da unidade não foram incluídos no custo operacional total da unidade, pois poderiam ser cobertos pela energia térmica produzida pela subunidade CHP. O custo da eletricidade foi fixado em 198 €/MWh de acordo com o fornecedor de energia elétrica grego.

Custo [€ / m³reator d] = Consumo de eletricidade [MWh / m³reator d] * pe [€ / MWh] + Depreciação [€ / m³reator d] --- **Equação 17**

Onde pe denota o preço da eletricidade de acordo com o fornecedor de energia. A receita da unidade foi assumida como proveniente da venda de eletricidade (Equação (18)). O preço de venda da eletricidade produzida a partir do biogás foi fixado em 204 €/MWhel, de acordo com a legislação grega [29].

Receita [€ / m³reator d] = Produtividade de Metano [m³ CH4 / m³reator d] * ηe [kWe / m³ CH4] * pb [€ / kWhe] --- **Equação 18**

Onde ηe representa a eficiência da unidade CHP em energia elétrica multiplicada pelo poder calorífico do metano, e pb denota o preço da energia elétrica a partir do biogás.

O processo de otimização começou considerando um valor inicial de HRT para cada razão de mistura de substrato. Subsequentemente, o conteúdo orgânico do efluente foi calculado, através do qual a produtividade do sistema foi estimada. O HRT ótimo para cada cenário foi estimado pelo algoritmo a fim de maximizar o lucro líquido da unidade (Equação (19)). Por outro lado, HRTs longos não foram favorecidos devido ao alto custo do equipamento e da energia necessária. Nesta direção, a função objetivo para maximização do lucro líquido da unidade para cada cenário de mistura é mostrada na Equação (19). A metodologia final para estimação do HRT para cada razão de substrato é apresentada na Fig. 3.

max (Receita - Custo) / HRT --- **Equação 19**

*(Fig. 3. Processo de otimização do HRT usando os resultados experimentais de sistemas em batelada para maximizar o lucro final de um sistema contínuo. Inclui um fluxograma mostrando o palpite inicial de HRT, cálculo de produtividade, função objetivo e decisão de otimização.)*

---

**3. Resultados e discussão**

**3.1. Treinamento do modelo - estimação dos parâmetros cinéticos**

Os resultados simulados do treinamento do modelo para os monosubstratos (OMW, CW e LCM) são apresentados na Fig. 4. O maior potencial metanogênico foi observado para o OMW, atingindo 820 NmL/g VSadicionado. Por outro lado, a maior taxa de produção foi observada para a digestão anaeróbia do LCM, possivelmente devido à concentração aumentada de nutrientes neste substrato, como nitrogênio. Os resultados de BMP do CW exibiram comportamento similar ao OMW, possivelmente devido às características similares de seu conteúdo orgânico (o teor de carboidratos totais do CW foi apenas 15% maior que o teor do OMW). O valor máximo do potencial de metano foi alcançado antes da marca de 70 dias para todos os experimentos, com o valor máximo de BMP do LCM sendo alcançado no dia 50. Por outro lado, apesar da maior taxa de produção de metano, o valor final de BMP para o LCM foi 25% menor que os monosubstratos de OMW e CW. Como pode ser observado na Fig. 4, o ajuste do modelo aos dados de monosubstrato foi muito satisfatório. Os parâmetros estimados para o modelo de Gompertz modificado (Equação (1)) durante esta etapa de treinamento do modelo estão resumidos na Tabela 2. Observou-se que não houve diferenças significativas entre os valores das taxas máximas de produção de metano. Este fato pode ser atribuído ao inóculo comum usado em todos os experimentos, pois muitos autores afirmam que a taxa de produção de metano é fortemente dependente da cultura microbiana utilizada [30-33].

**Tabela 2**
Valores dos parâmetros estimados para a equação de Gompertz modificada, otimizada com os monosubstratos (OMW, CW, LCM).

| Parâmetro | Unidades           | OMW        | CW         | LCM        |
| :-------- | :----------------- | :--------- | :--------- | :--------- |
| BMP       | NmL CH4/g VS       | 896 ± 18   | 721 ± 4    | 597 ± 5    |
| Rm        | NmL CH4/g VS/d     | 20 ± 1     | 19 ± 1     | 21 ± 1     |
| lag       | d                  | 14 ± 1     | 13 ± 1     | 4 ± 1      |

*(Fig. 4. Rendimento de metano para testes BMP de OMW (a), CW (b) e LCM (c). A linha sólida representa os dados simulados do modelo, enquanto o gráfico de dispersão representa os pontos experimentais.)*

Os parâmetros de Gompertz da Tabela 2 para o substrato bruto foram mantidos constantes para o treinamento do modelo dos coeficientes de sinergia usando dados de co-digestão. Inicialmente, um conjunto diferente de parâmetros de sinergia foi estimado para cada conjunto de dados de misturas de substratos, seguido pela modelagem dos parâmetros de sinergia usando equações empíricas para ajustar os diferentes conjuntos estimados. A Fig. 5 ilustra as curvas de produção de metano da co-digestão de OMW com LCM. A inibição da taxa de produção de metano foi provavelmente devido à maior concentração inicial de fenóis na mistura. De acordo com Gelegenis et al., a co-digestão de OMW com outros resíduos alivia o efeito de fatores inibitórios [34]. Angelidaki e Ahring demonstraram que a falta de amônia, necessária como fonte de nitrogênio para a síntese de biomassa bacteriana e como um importante tampão de pH, poderia ser responsável pelos problemas encontrados durante a degradação anaeróbia do OMW, enquanto a amônia faltante poderia ser fornecida por esterco bovino (CM) ou efluente de suinocultura durante a co-degradação de OMW e esterco [35]. Este fato foi demonstrado pelo aumento da taxa máxima de produção para 50 NmL CH4/g VS/d para o cenário de OMW:LCM igual a 50:50 comparado à taxa do cenário de monosubstrato OMW (20 NmL CH4/g VS/d).

Os resultados da co-digestão de CW e LCM são apresentados na Fig. 6. A combinação de CW e LCM resultou em alta atividade dos microrganismos metanogênicos. Uma taxa de produção maior foi observada usando a mistura com uma razão 50:50 de CW:LCM (55 NmL/g VS/d comparado a 35 NmL/g VS/d para as outras misturas CW:LCM). Esta taxa maior pode ser explicada pela alta contribuição do LCM na mistura, que é um substrato rico em nitrogênio. No processo de co-digestão com substratos altamente biodegradáveis, como o CW, a amônia contida no esterco animal poderia passar de uma causa de inibição [36] para um elemento positivo para o processo biológico, pois a amônia pode fornecer a capacidade tampão necessária [37]. Além disso, vários estudos demonstraram que a co-digestão de CW com LCM pode manter pH favorável e melhorar a produção de biogás [38].

Misturar OMW com outros resíduos oferece várias vantagens, como redução da COD da alimentação e da concentração de fenóis totais, sem necessidade de adicionar nutrientes (i.e., nitrogênio e fósforo) se o OMW for misturado com resíduos ricos em nutrientes, e a possibilidade de operar uma planta de tratamento durante todo o ano com base na co-digestão de efluentes gerados sazonalmente [39]. A co-digestão de OMW com CW também foi estudada para avaliar o desempenho em termos de produtividade e o papel da co-digestão (Fig. 7). Exibiu-se que há um aumento significativo da taxa de produção de metano com o aumento de CW na mistura.

Além disso, a co-digestão de OMW com LCM e CW foi realizada para observar o desempenho do processo com uma mistura de três monosubstratos (Fig. 8). Observou-se que a produção máxima foi alcançada em 35 dias. A menor produtividade entre a co-digestão de OMW, CW e LCM foi observada usando a mistura de OMW:CW:LCM igual a 25:25:50, atingindo o valor de 800 NmL/g VS.

*(Fig. 5. Rendimento de metano para testes BMP das misturas com razão OMW:LCM = 75:25 (a), OMW:LCM = 50:50 (b) e OMW:LCM = 25:75 (c). A linha sólida representa os dados simulados do modelo, enquanto o gráfico de dispersão representa os pontos experimentais.)*

*(Fig. 6. Rendimento de metano para testes BMP das misturas com razão CW:LCM = 75:25 (a), CW:LCM = 50:50 (b) e CW:LCM = 25:75 (c). A linha sólida representa os dados simulados do modelo, enquanto o gráfico de dispersão representa os pontos experimentais.)*

*(Fig. 7. Rendimento de metano para testes BMP das misturas com razão OMW:CW = 75:25 (a), OMW:CW = 50:50 (b) e OMW:CW = 25:75 (c). A linha sólida representa os dados simulados do modelo, enquanto o gráfico de dispersão representa os pontos experimentais.)*

*(Fig. 8. Rendimento de metano para testes BMP das misturas com razão OMW:CW:LCM = 50:25:25 (a), OMW:CW:LCM = 25:25:50 (b) e OMW:CW:LCM = 25:50:25 (c). A linha sólida representa os dados simulados do modelo, enquanto o gráfico de dispersão representa os pontos experimentais.)*

Após o cálculo dos parâmetros de sinergia para cada cenário, considerou-se necessário correlacionar os resultados obtidos com a razão de mistura dos substratos. Por esta razão, certas equações algébricas empíricas foram usadas para descrever o comportamento dos parâmetros de sinergia em função da composição do substrato. As equações que foram usadas podem não ter significado físico, mas poderiam descrever os efeitos de sinergia em cada mistura dentro da faixa dos conjuntos de dados experimentais. As equações para cada parâmetro são apresentadas nas equações (20)-(22). Essas equações foram escolhidas de acordo com os parâmetros estatísticos R² e valor-p para as diferentes formas de equação do software Minitab. Apenas os termos com diferença estatística significativa foram implementados no modelo.

SnBMP = 0.98 XOMW + 1.06 XCW + 0.99 XLCM + 3.21 XOMW XLCM + 3.75 XCW XLCM --- **Equação 20**

SNRm = 0.94 XOMW + 1.09 XCW + 1.01 XLCM + 6.33 XOMW XLCM + 6.83 XCW XLCM --- **Equação 21**

Snlag = 0.99 XOMW + 1.05 XCW + 0.97 XLCM + 5.77 XOMW XCW (XOMW - XCW) --- **Equação 22**

Onde XOMW, XCW e XLCM representam a porcentagem de cada substrato na mistura em termos de VS.

Os resultados da modelagem matemática das diferentes misturas foram agrupados em gráficos ternários (Fig. 9). Observa-se que duas áreas diferentes com valores máximos de BMP apareceram (Fig. 9a). No gráfico ternário de sinergia (Fig. 9b), a mistura de CW: LCM igual a 50:50 parece ter o maior efeito de sinergia em termos de produtividade de metano. Este fato pode ocorrer devido à alta complementaridade dos substratos em relação à sua grande diferença na concentração de carboidratos e nitrogênio total. Na mesma direção, uma área com a taxa máxima foi observada perto da razão de mistura de CW: LCM igual a 50:50 com o efeito de sinergia mostrando o mesmo comportamento.

*(Fig. 9. Gráficos ternários do potencial de metano [mL CH4/g VSadicionado] (a), efeito de sinergia no potencial de metano (SnBMP) (b), taxa máxima de produção de metano [mL CH4/g VSadicionado/d] (c), e efeito de sinergia na taxa máxima de produção de metano (SnRm) (d) para as diferentes razões de mistura de OMW, CW e LCM.)*

**3.2. Projeto da planta - tomada de decisão**

As equações empíricas extraídas dos dados experimentais foram usadas para o desenvolvimento de um algoritmo de otimização que seleciona um projeto ótimo da planta de digestão anaeróbia para as diferentes cenários de mistura. O algoritmo otimizou o valor de HRT para cada mistura e estimou o lucro máximo para a planta específica usando a função de otimização (Equação (19)). A estimação dos HRTs ótimos é representada na Fig. 10a. Ficou claro que HRTs mais baixos levam a custos de capital menores devido ao menor tamanho do equipamento, bem como menor custo operacional (energia necessária para aquecimento e agitação por m³ de substrato). Por outro lado, HRTs muito baixos limitam o metano recuperável do substrato e, como resultado, o lucro obtido. A seleção do melhor cenário operacional torna-se mais clara observando o gráfico ternário do lucro máximo para cada cenário em termos de €/m³reator/d (Fig. 10b). O melhor cenário apareceu na área da razão OMW: LCM de 70:30. Duas outras regiões para uma unidade lucrativa foram observadas (CW: LCM igual a 65:35 e OMW:CW: LCM igual a 40:50:10). Esses resultados estão na mesma direção que os relatados por outros autores. No trabalho de [40], a co-digestão de OMW com esterco líquido de aves com uma razão de mistura de 70:30 mostrou a produtividade máxima de metano entre outras razões de mistura. Os autores mencionaram que este fato ocorre devido à razão COD/N que foi igual a 50,7. Além disso, no trabalho referente à co-digestão anaeróbia de CW com esterco bruto (RM) [41], houve uma tendência de aumentar a sustentabilidade do investimento aumentando a porcentagem de CW na mistura, com a maximização sendo alcançada para a razão de mistura de CW:RM igual a 70:30. Este resultado está em linha com os resultados deste trabalho, observando que o processo de co-digestão de CW e LCM foi mais lucrativo aumentando o CW na mistura.

Além disso, a análise mostra que uma planta com apenas LCM como alimentação é menos sustentável nesta capacidade específica de planta. Este fato está em linha com a baixa quantidade de biometano produzida no teste de BMP. Este fato pode ocorrer devido ao baixo rendimento de metano do esterco animal como único afluente da AD, conforme relatado na literatura [42]. Na maioria dos casos, este tipo de resíduo é usado como co-substrato em AD para aumento do teor de umidade e uso da capacidade tampão. Além disso, este resíduo poderia diluir resíduos concentrados para permitir o suprimento periódico de resíduos na planta [43].

*(Fig. 10. Gráficos ternários do HRT ótimo em [d] (a) e lucro líquido ótimo [€/m³reator/d] (b) para as diferentes razões de mistura dos monosubstratos (OMW, CW e LCM).)*

---

**4. Conclusões**

Em conclusão, OMW, CW e LCM são subprodutos que criam questões ambientais e sociais significativas nos países mediterrâneos. Esses tipos de correntes de resíduos provaram ser substratos adequados para produção de energia via digestão anaeróbia. O efeito de sinergia foi observado e quantificado através do desenvolvimento do modelo usando a equação de Gompertz. Através da análise proposta, exibiu-se que a complementaridade das características do substrato pode ser a principal razão para o efeito de sinergia na produção de biogás. A análise dos resultados da modelagem mostra que o LCM pode ser um co-substrato muito útil para o aumento do rendimento de metano em um sistema em batelada. O maior rendimento de metano foi alcançado na mistura OMW: LCM igual a 70:30. Em relação à modelagem do processo, exibiu-se que todo o processo de co-digestão pode ser facilmente descrito por equações algébricas em condições de estado estacionário, visando a aplicabilidade mais ampla do modelo. A análise apresentada aqui pode ser expandida e aprimorada incorporando dados de sistema contínuo para validação do modelo, enquanto modelos mais complexos de digestão anaeróbia, como o ADM1, podem ter mérito no escopo de melhorar a precisão do modelo (mas também a complexidade do modelo). Finalmente, a análise proposta pode ser usada para guiar a investigação experimental em sistemas contínuos e pode ser uma ferramenta simples e útil para o projeto de plantas de processos contínuos em escala real e tomada de decisão para as condições ótimas de operação para maximizar a sustentabilidade econômica do processo.

---

**Financiamento**

Esta pesquisa foi cofinanciada pela União Europeia e por fundos nacionais gregos através do Programa Operacional Competitividade, Empreendedorismo e Inovação 2014-2020 (EPAnEK), sob a chamada PESQUISA - CRIA – INOVA através do projeto "Desenvolvimento de um sistema integrado inovador para estimar o potencial metanogênico bioquímico (BMP) de diferentes fontes de biomassa - Green.BMP" (código do projeto: T1EDK-03148).

---

**Declaração de contribuição de autoria CRediT**

**Georgios Manthos:** Curadoria de dados, Software, Investigação, Análise formal, Metodologia, Validação, Redação - rascunho original. **Margarita Dareioti:** Conceituação, Investigação, Curadoria de dados, Validação. **Dimitris Zagklis:** Metodologia, Software, Análise formal, Validação, Visualização, Redação - revisão e edição. **Michael Kornaros:** Recursos, Supervisão, Administração do projeto, Aquisição de financiamento.

---

**Declaração de interesse concorrente**

Os autores declaram que não possuem interesses financeiros concorrentes conhecidos ou relacionamentos pessoais que possam ter parecido influenciar o trabalho relatado neste artigo.

---

**Referências**

[1] L.C. Freitas, J.R. Barbosa, A.L.C. da Costa, F.W.F. Bezerra, R.H.H. Pinto, R.N. de Carvalho Junior, From waste to sustainable industry: how can agro-industrial wastes help in the development of new products? Resour. Conserv. Recycl. 169 (2021), 105466.
[2] S. Kumar, H.V. Bhati, Waste management to zero waste: global perspectives and review of Indian law and policy, Emerg. Trends to Approaching Zero Waste (2022) 79-101.
[3] P. McKendry, Energy production from biomass (part 2): conversion technologies, Bioresour. Technol. 83 (2002) 47-54.
[4] A.M. Petersen, O. V Okoro, F. Chireshe, T. Moonsamy, J.F. Görgens, Systematic cost evaluations of biological and thermochemical processes for ethanol production from biomass residues and industrial off-gases, Energy Convers. Manag. 243 (2021), 114398.
[5] T.D. Foust, A. Aden, A. Dutta, S. Phillips, An economic and environmental comparison of a biochemical and a thermochemical lignocellulosic ethanol conversion processes, Cellulose 16 (2009) 547-565.
[6] C. Mao, Y. Feng, X. Wang, G. Ren, Review on research achievements of biogas from anaerobic digestion, Renew. Sustain. Energy Rev. 45 (2015) 540-555, https://doi.org/10.1016/j.rser.2015.02.032.
[7] K. Tsigkou, P. Tsafrakidou, A. Kopsahelis, D. Zagklis, C. Zafiri, M. Kornaros, Used disposable nappies and expired food products valorisation through one-& two-stage anaerobic co-digestion, Renew. Energy 147 (2020) 610-619.
[8] K.F. Adekunle, J.A. Okolie, A review of biochemical process of anaerobic digestion, Adv. Biosci. Biotechnol. 6 (2015) 205.
[9] M.N.I. Siddique, Z.A. Wahid, Achievements and perspectives of anaerobic co-digestion: a review, J. Clean. Prod. 194 (2018) 359-371.
[10] K. Tsigkou, D. Zagklis, P. Tsafrakidou, P. Zapanti, G. Manthos, K. Karamitou, C. Zafiri, M. Kornaros, Expired food products and used disposable adult nappies mesophilic anaerobic co-digestion: biochemical methane potential, feedstock pretreatment and two-stage system performance, Renew. Energy 168 (2021) 309-318.
[11] J. Kim, G. Baek, J. Kim, C. Lee, Energy production from different organic wastes by anaerobic co-digestion: maximizing methane yield versus maximizing synergistic effect, Renew. Energy 136 (2019) 683-690.
[12] D. Poggio, M. Walker, W. Nimmo, L. Ma, M. Pourkashanian, Modelling the anaerobic digestion of solid organic waste-Substrate characterisation method for ADM1 using a combined biochemical and kinetic parameter estimation approach, Waste Manag. 53 (2016) 40-54.
[13] B. Velázquez-Martí, O.W. Meneses-Quelal, J. Gaibor-Chavez, Z. Niño-Ruiz, Review of mathematical models for the anaerobic digestion process, in: Anaerob. Dig., IntechOpen, 2018.
[14] K. Rajendran, G.S. Murthy, Techno-economic and life cycle assessments of anaerobic digestion-A review, Biocatal. Agric. Biotechnol. 20 (2019), 101207.
[15] J. Vasco-Correa, S. Khanal, A. Manandhar, A. Shah, Anaerobic digestion for bioenergy production: global status, environmental and techno-economic implications, and government policies, Bioresour. Technol. 247 (2018) 1015-1026.
[16] G. Redman, A Detailed Economic Assessment of Anaerobic Digestion Technology and its Suitability to UK Farming and Waste Systems, Andersons Cent. Leicestershire, UK, 2010.
[17] A.D. Eaton, L.S. Clesceri, A.E. Greenberg, M.A.H. Franson, Standard Methods for the Examination of Water and Wastewater, twenty-second ed., APHA, Washingt. DC, 2012.
[18] B. Joseffson, Rapid spectrophotometric determination of total carbohydrates, in: K. Grasshoff, M. Ehrhardt, K. Kremling (Eds.), Methods Seawater Anal, Verlag Chemie GmbH, Weinheim, Ger, 1983, pp. 340-342.
[19] G. Manthos, D. Zagklis, K. Mesisklis, M. Kornaros, Effect of two-phase olive pomace acidification on odor prevention and kernel oil acidity reduction as a function of storage duration, J. Environ. Manag. 298 (2021), 113453.
[20] P.G. Waterman, S. Mole, Analysis of Phenolic Plant Metabolites, Wiley, 1994.
[21] C. Holliger, M. Alves, D. Andrade, I. Angelidaki, S. Astals, U. Baier, C. Bougrier, P. Buffière, M. Carballa, V. De Wilde, Towards a standardization of biomethane potential tests, Water Sci. Technol. 74 (2016) 2515-2522.
[22] W.F. Owen, D.C. Stuckey, J.B. Healy Jr., L.Y. Young, P.L. McCarty, Bioassay for monitoring biochemical methane potential and anaerobic toxicity, Water Res. 13 (1979) 485-492.
[23] P. Tsafrakidou, G. Manthos, D. Zagklis, J. Mema, M. Kornaros, Assessment of substrate load and process pH for bioethanol production-Development of a kinetic model, Fuel 313 (2022), 123007.
[24] C. Zhang, G. Xiao, L. Peng, H. Su, T. Tan, The anaerobic co-digestion of food waste and cattle manure, Bioresour. Technol. 129 (2013) 170-176.
[25] A. Rabii, S. Aldin, Y. Dahman, E. Elbeshbishy, A review on anaerobic co-digestion with a focus on the microbial populations and the effect of multi-stage digester configuration, Energies 12 (2019) 1106.
[26] D.J. Batstone, J. Keller, I. Angelidaki, S. V Kalyuzhnyi, S.G. Pavlostathis, A. Rozzi, W.T.M. Sanders, H.A. Siegrist, V.A. Vavilin, The IWA anaerobic digestion model no 1 (ADM1), Water Sci. Technol. 45 (2002) 65-73, https://doi.org/10.2166/wst.2002.0292.
[27] K.M. Guthrie, Data and techniques for preliminary capital cost estimating, Chem (1969).
[28] Energy Solutions Center. https://understandingchp.com/chp-applications-guide/6-8-rules-of-thumb-for-chp-engineering-and-installation-costs/, 2022.
[29] Greek Law 4414/2016, New Aid Scheme for Power Plants Using RES and Co-generation of Electricity and High-Efficiency Heat, 2016. https://cdn.climatepolicyradar.org/navigator/GRC/2016/law-4414-2016_59c2a9daa5f23c5fedb3a2568c2670c0.pdf.
[30] J. Ma, C. Frear, Z. Wang, L. Yu, Q. Zhao, X. Li, S. Chen, A simple methodology for rate-limiting step determination for anaerobic digestion of complex substrates and effect of microbial community ratio, Bioresour. Technol. 134 (2013) 391-395.
[31] V. Córdoba, M. Fernández, E. Santalla, The effect of substrate/inoculum ratio on the kinetics of methane production in swine wastewater anaerobic digestion, Environ. Sci. Pollut. Res. 25 (2018) 21308-21317.
[32] V. Córdoba, M. Fernández, E. Santalla, The effect of different inoculums on anaerobic digestion of swine wastewater, J. Environ. Chem. Eng. 4 (2016) 115-122.
[33] F. Ali Shah, Q. Mahmood, M. Maroof Shah, A. Pervez, S. Ahmad Asad, Microbial ecology of anaerobic digesters: the key players of anaerobiosis, Sci. World J. (2014), 2014.
[34] J. Gelegenis, D. Georgakakis, I. Angelidaki, V. Mavris, Optimization of biogas production by co-digesting whey with diluted poultry manure, Renew. Energy 32 (2007) 2147-2160.
[35] I. Angelidaki, B.K. Ahring, Codigestion of olive oil mill wastewaters with manure, household waste or sewage sludge, Biodegradation 8 (1997) 221-226.
[36] O. Yenigün, B. Demirel, Ammonia inhibition in anaerobic digestion: a review, Process Biochem. 48 (2013) 901-911.
[37] J. Procházka, P. Dolejš, J. Máca, M. Dohányos, Stability and inhibition of anaerobic processes caused by insufficiency or excess of ammonia nitrogen, Appl. Microbiol. Biotechnol. 93 (2012) 439-447.
[38] E. Comino, V.A. Riggio, M. Rosso, Biogas production by anaerobic co-digestion of cattle slurry and cheese whey, Bioresour. Technol. 114 (2012) 46-53.
[39] D. Mantzavinos, N. Kalogerakis, Treatment of olive mill effluents: Part I. Organic matter degradation by chemical and biological processes an overview, Environ. Int. 31 (2005) 289-295, https://doi.org/10.1016/j.envint.2004.10.005.
[40] S. Khoufi, A. Louhichi, S. Sayadi, Optimization of anaerobic co-digestion aof olive mill wastewater and liquid poultry manure in batch condition and semi-continuous jet-loop reactor, Bioresour. Technol. 182 (2015) 67-74.
[41] S.M. Imeni, L. Pelaz, C. Corchado-Lopo, A.M. Busquets, S. Ponsá, J. Colón, Techno-economic assessment of anaerobic co-digestion of livestock manure and cheese whey (Cow, Goat & Sheep) at small to medium dairy farms, Bioresour. Technol. 291 (2019), 121872.
[42] L. Zhang, Y.-W. Lee, D. Jahng, Anaerobic co-digestion of food waste and piggery wastewater: focusing on the role of trace elements, Bioresour. Technol. 102 (2011) 5048-5059.
[43] I. Angelidaki, L. Ellegaard, Codigestion of manure and organic wastes in centralized biogas plants, Appl. Biochem. Biotechnol. 109 (2003) 95-105.

---