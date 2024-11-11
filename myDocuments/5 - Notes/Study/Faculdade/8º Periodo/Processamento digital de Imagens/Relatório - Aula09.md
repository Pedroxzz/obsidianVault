---
Index: "[[Processamento digital de Imagens]]"
---
1) Compare e explique os resultados obtidos entre a imagem original e a  
Transformação de Negativo.  
Transformação de Negativo:  
• A transformação de negativo é realizada subtraindo o valor de cada pixel de 255.  
Isso inverte os tons da imagem: áreas claras tornam-se escuras e vice-versa.  
• Resultados: Se a imagem original contém áreas claras (como ossos em uma  
radiografia), na imagem negativa essas áreas se tornarão escuras. Isso pode  
ajudar a realçar detalhes em regiões que são menos visíveis na imagem original,  
facilitando a análise.  
2) Compare e explique os resultados obtidos entre a imagem original e a

Transformação Logarítmica com c = 0.01, c = 0.05, c = 0.1, c =0.25, c = 0.5, c = 0.75, c  
= 1, c = 1.5, c = 2 e c = 3.  
Transformação Logarítmica:  
• A transformação logarítmica é usada para aumentar o contraste em regiões  
escuras da imagem. O parâmetro ccc controla a intensidade da transformação.  
• Resultados para diferentes valores de ccc:  
o c = 0.01 a c = 0.05: A imagem pode parecer um pouco mais clara, mas o  
contraste não é muito pronunciado.  
o c = 0.1 a c = 0.25: O contraste aumenta, revelando mais detalhes nas  
regiões escuras.  
o c = 0.5 a c = 0.75: A imagem se torna bastante clara, e os detalhes  
começam a ser mais visíveis.  
o c = 1 a c = 1.5: As áreas escuras são muito mais realçadas, permitindo  
observar características sutis.  
o c = 2 a c = 3: A imagem pode se tornar excessivamente clara, resultando  
em perda de informações em áreas que eram originalmente claras. O  
destaque excessivo pode mascarar detalhes importantes.  
o

3) Compare e explique os resultados obtidos entre a imagem original e a  
Transformação Logarítmica para os seguintes casos:  
a) c=1,γ=1c = 1, \gamma = 1c=1,γ=1 e diferentes valores de ε\epsilonε:  
• ε=0\epsilon = 0ε=0: Normalização padrão sem adição de valor, a  
transformação é simples.  
• ε=0.5\epsilon = 0.5ε=0.5 a ε=2\epsilon = 2ε=2: A adição de ε\epsilonε desloca  
a imagem, permitindo que pixels mais escuros ganhem um valor mínimo antes  
de serem transformados. Com valores maiores de ε\epsilonε, mais detalhes nas  
áreas escuras podem ser revelados, mas também pode causar perda de  
informações em áreas claras se o deslocamento for muito grande.  
b) c=1,ε=0c = 1, \epsilon = 0c=1,ε=0 e diferentes valores de γ\gammaγ:  
• γ=0\gamma = 0γ=0: A imagem se torna uma constante, resultando em uma  
imagem uniforme.  
• γ=0.5\gamma = 0.5γ=0.5: O contraste é aumentado para tons mais escuros,  
mas as áreas claras começam a ser mais visíveis também.  
• γ=1\gamma = 1γ=1: A transformação é idêntica à transformação logarítmica  
padrão.

• γ=1.5\gamma = 1.5γ=1.5 e γ=2\gamma = 2γ=2: O contraste em áreas escuras  
aumenta, resultando em mais detalhes visíveis, mas pode levar a saturação em  
áreas mais claras.  
c) c=0.5,ε=0.2,γ=0.5c = 0.5, \epsilon = 0.2, \gamma = 0.5c=0.5,ε=0.2,γ=0.5:  
• Este conjunto de parâmetros resultará em uma imagem onde as áreas escuras  
são mais ressaltadas, mas ainda há alguma leveza nas áreas claras. O uso de  
c=0.5c = 0.5c=0.5 e γ=0.5\gamma = 0.5γ=0.5 permitirá que detalhes sutis em  
áreas escuras sejam mais evidentes sem perder totalmente as informações em  
regiões mais claras.