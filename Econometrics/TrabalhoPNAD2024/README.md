## Etapas do Trabalho

### Q1:
Primeiramente, vocês devem acessar os dados da PNAD referente à cross-section do seu grupo. Isso pode ser feito diretamente pelo site, ou através do pacote `pnadcibge` no R. Em todos os casos, utilizem os dados referentes ao terceiro trimestre da amostra.

### Q2:
A PNAD possui uma quantidade enorme de dados, porém iremos utilizar apenas algumas variáveis tradicionais da literatura. Como o dataset guarda os dados através de seus códigos, vocês precisam consultar o dicionário da PNAD (disponível no site) e selecionar as colunas com os códigos corretos. As variáveis são:

- Rendimento mensal efetivo de todos os trabalhos para pessoas de 14 anos ou mais de idade;
- Horas habitualmente trabalhadas em todos os trabalhos para pessoas de 14 anos ou mais;
- Unidade da Federação;
- Rural/Urbano;
- Sexo;
- Idade do morador na data de referência;
- Cor ou raça;
- Curso mais elevado que frequentou anteriormente?;
- Anos de estudo;
- Condição em relação à força de trabalho na semana de referência para pessoas de 14 anos ou mais de idade;
- Condição de ocupação na semana de referência para pessoas de 14 anos ou mais de idade;
- Setor do trabalho.

### Q3:
Baixadas as variáveis, tomem cuidado para realizar quaisquer limpezas que possam ser necessárias. Todas as informações sobre valores de variáveis estão disponíveis no dicionário.

### Q4:
Filtre a base de dados, mantendo apenas a população entre 20 e 60 anos. Calcule a proporção de pessoas economicamente ativas, condicional ao nível de escolaridade, sexo e idade, separadamente. Depois, façam o mesmo exercício apenas para a região de vocês (Amapá). Como a probabilidade de estar no mercado de trabalho varia em função dessas características? Analisem também as possíveis causas de diferenças entre o resultado nacional e o resultado específico do grupo.

### Q5:
Após gerar a base tratada, filtre os dados para manter apenas trabalhadores do setor privado, empregados na data da amostra. Vocês devem reportar uma tabela com estatísticas descritivas (mínimo, máximo, média, desvio-padrão e quantis) das variáveis contínuas, e as proporções de cada grupo para as variáveis de nível (trate idade como contínua). Para realizar nossa avaliação, é importante que nenhuma variável tenha todas as observações iguais. Explique qual seria o problema caso contrário.

### Q6:
Calcule o salário de cada indivíduo e gere os histogramas dos salários condicionais ao seu nível mais elevado de educação. Faça o mesmo com o logaritmo dos salários. Qual conjunto de histogramas mais se assemelha com uma distribuição normal? Comente a relação desses histogramas com o que sabemos sobre a distribuição condicional de 𝑦 dadas todas as hipóteses de MQO.

### Q7:
Faça uma regressão simples do logaritmo dos salários sobre anos de escolaridade e reporte o resultado, comentando os testes de hipótese usuais. Se estiver usando o R, o pacote `stargazer` pode ser útil para a geração de tabelas.

### Q8:
Faça duas regressões simples, de anos de escolaridade sobre sexo e raça, respectivamente. O que os resultados dessa regressão nos dizem sobre a validade da regressão feita no item anterior? Analise o possível viés que pode existir, se baseando na teoria de MQO, e a direção desse viés.

### Q9:
Faça duas regressões, de logaritmo dos salários sobre anos de educação, sendo uma apenas com mulheres e outra apenas com homens. Os coeficientes estimados são os mesmos? O que isso nos diz sobre o que precisamos incluir na regressão completa? Além do modelo, vocês devem gerar um gráfico com os pontos da amostra (ou uma subamostra deles, se o código ficar lento), e as duas retas de regressão.

### Q10:
Com base na sua conclusão do item anterior, façam uma regressão para explicar o logaritmo dos salários, incluindo todas as variáveis vistas até aqui, e interpretem os valores dos coeficientes estimados, assim como a significância deles e de quaisquer interações incluídas. Qual é o valor marginal de um ano adicional de escolaridade para um homem? E para uma mulher? Eles são estatisticamente iguais?

### Q11:
É possível que o nível de experiência tenha efeito importante sobre os salários, porém há dúvidas sobre como deve ser a forma funcional desse efeito. Como poderíamos incorporar efeitos não-lineares no modelo? Supondo que o efeito seja quadrático, qual seria o nível de experiência que maximiza o salário, tudo mais constante?

### Q12 (Bônus):
Para finalizar, comentem como os resultados podem se relacionar com as probabilidades de estar no mercado de trabalho calculadas no começo do trabalho. A análise feita aqui é apenas sobre salários reais, ou seja, pode existir um viés de seleção sobre a amostra de salários, dado que as pessoas decidem trabalhar em função de suas características pessoais, que são também as variáveis que usamos na regressão. Isso pode ser interpretado como considerar o salário de reserva de um indivíduo uma função de suas características. Como vocês esperariam que o salário de reserva varie com idade, sexo e escolaridade? Como essa variação pode gerar viés no modelo? Este item é inteiramente opcional.

