<h1>Projeto: Cálculo de Raízes de Equação do 2º Grau</h1> <h2>Descrição</h2>
Este projeto em Java realiza o cálculo das raízes de uma equação do segundo grau (ax² + bx + c = 0).
O sistema trata situações em que:

Existem duas raízes reais diferentes

Existe uma raiz real (raiz dupla)

Não existem raízes reais (delta negativo)

O tratamento é feito utilizando:

<b>Exceções Checadas</b> (checked exceptions)

<b>Exceções Não Checadas</b> (runtime exceptions)

<h2>Estrutura das Classes</h2> <h3>AulaPratica</h3> Classe principal que realiza: - Leitura dos coeficientes <b>a</b>, <b>b</b> e <b>c</b>. - Cálculo das raízes usando métodos com exceções checadas e não checadas. - Exibição dos resultados ou mensagens de erro.
<b>Principais métodos:</b>

<code>lerValor(Scanner, String)</code>: Lê um número real com tratamento de entrada inválida.

<h3>Equacao</h3> Classe auxiliar que contém métodos para o cálculo das raízes:
<b>Métodos:</b>

<code>raizEq2GrauX1(double a, double b, double c)</code>: Retorna a primeira raiz (exceção checada).

<code>raizEq2GrauX2(double a, double b, double c)</code>: Retorna a segunda raiz (exceção checada).

<code>raizEq2GrauX1_RT(double a, double b, double c)</code>: Retorna a primeira raiz (exceção não checada).

<code>raizEq2GrauX2_RT(double a, double b, double c)</code>: Retorna a segunda raiz (exceção não checada).

<h3>NaoTemRaizesReaisException</h3> Classe que representa uma exceção checada lançada quando o delta é negativo. <h3>NaoTemRaizesReaisRuntimeException</h3> Classe que representa uma exceção não checada lançada quando o delta é negativo. <h2>Execução</h2>
No método <code>main</code> da classe <code>AulaPratica</code>:

O programa pede para o usuário informar os coeficientes da equação.

Calcula as raízes utilizando métodos com e sem exceções checadas.

Exibe os valores das raízes no console ou informa se não existem raízes reais.

<h2>Exemplos de Teste</h2> <h3>Exemplo 1 — Delta Positivo</h3>
<b>Entrada:</b>

<pre> a = 1 b = -5 c = 6 </pre>
<b>Saída:</b>

<pre> Raiz x1: 3.0 Raiz x2: 2.0 Raiz x1 (Runtime): 3.0 Raiz x2 (Runtime): 2.0 </pre> <h3>Exemplo 2 — Delta Zero</h3>
<b>Entrada:</b>

<pre> a = 1 b = -4 c = 4 </pre>
<b>Saída:</b>

<pre> Raiz x1: 2.0 Raiz x2: 2.0 Raiz x1 (Runtime): 2.0 Raiz x2 (Runtime): 2.0 </pre> <h3>Exemplo 3 — Delta Negativo</h3>
<b>Entrada:</b>

<pre> a = 1 b = 1 c = 1 </pre>
<b>Saída:</b>

<pre> Não existem raízes para essa equação. Não existem raízes reais para esta equação (Runtime). </pre> <h2>Observações</h2>
O projeto é uma simulação didática para aprendizado sobre:

Manipulação de exceções (checked e unchecked).

Cálculo de raízes de equações de 2º grau.

O programa faz tratamento de entradas inválidas.

Todos os métodos de cálculo validam se o <code>delta</code> é negativo antes de tentar calcular a raiz quadrada.

<h2>Tecnologias</h2>
Java 8+

Scanner para entrada de dados

Tratamento de Exceções

<h2>Autor</h2>
Desenvolvido por <b>Murilo Oliveira</b>.
