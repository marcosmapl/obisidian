
**COVARIÂNCIA**

- Desvio padrão e a variância são duas medidas de dispersão aplicadas quando temos uma **única variável aleatória.** Elas medem o desvio em torno da média.  
- A covariância tem por objetivo **avaliar os desvios conjuntos de duas variáveis aleatórias.**

$$ VAR(X) = E[(X_i - \bar{X})^2] = \frac{1}{n} \cdot \sum_{i=1}^n{(X_i - \bar{X})^2} $$
​
$$ VAR(Y) = E[(Y_i - \bar{Y})^2] = \frac{1}{n} \cdot \sum_{i=1}^n{(Y_i - \bar{Y})^2} $$​

$$ COV(X,Y) = E[(X_i - \bar{X})(Y_i - \bar{Y})] = \frac{1}{n} \cdot \sum_{i=1}^n{(X_i - \bar{X})(Y_i - \bar{Y})} $$​
$$ r = \frac{COV(X,Y)}{\sigma_X \cdot \sigma_Y} = \frac{\sum_{i=1}^n{(X_i - \bar{X})(Y_i - \bar{Y})}}{ \sqrt{ \sum_{i=1}^n{(X_i - \bar{X})^2}  \cdot \sum_{i=1}^n{(Y_i - \bar{Y})^2} }} $$


- ⚠️ Também é importante que você saiba: a correlação mede a relação linear entre duas variáveis, mas não significa que a variação de uma cause a variação da outra. É possível ainda que dois eventos tenham uma forte correlação mesmo sem causalidade nem causa em comum. Simplesmente por acaso. São as chamadas “correlações espúrias”.

**2.1 Propriedades do Coeficiente de Correlação**

- **1ª Propriedade**: o coeficiente de correlação não sofre alteração quando uma constante é adicionada a (ou subtraída de) uma variável.  
- **2ª Propriedade:** o coeficiente de correlação pode não sofrer alteração ou pode ter seu sinal alterado quando uma variável é multiplicada (ou dividida) por uma constante. Caso as constantes tenham o mesmo sinal, o valor do coeficiente de correlação não será alterado. Por outro lado, se as constantes tiverem sinais contrários, o coeficiente mudará de sinal, mas o valor permanecerá inalterado.

❗Veja como a banca cobrou essa tópico na⚡ **Questão** **[#674344](https://www.tecconcursos.com.br/questoes/674344)**