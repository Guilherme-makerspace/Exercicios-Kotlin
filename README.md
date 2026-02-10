# ***Exercicios-Kotlin***

## ***Estrutura Sequencial***

### *Exercicio 1*
```kotlin
fun main() {
    var entradaCelsius = readln()
    	//F = C * 9/5 + 32
    val saidaFahrenheit = entradaCelsius.toInt() * 9/5 + 32
    
    println(saidaFahrenheit)
}
```
### *Exercicio 2*
```kotlin
  fun main() {
    var entradaFahrenheit = readln()
    	// C = (F - 32) * 5/9
    val saidaCelsius = (entradaFahrenheit.toInt() - 32) * 5/9
    
    println(saidaCelsius)
}
```
### *Exercicio 3*
```kotlin
fun main() {
    val pi = 3.14159
    var raio = readln()
    var altura = readln()
 	var volumeLata = pi * (raio.toInt() * raio.toInt()) * altura.toInt()
    
     // V = π * raio^2 * altura
     
    println(volumeLata)
}
```
### *Exercicio 4*
```kotlin
fun main() {
    var distancia = readln()
    var consumo = readln()
    var litros = distancia.toInt() / consumo.toInt()
    // litros = distância / consumo
    println(litros)
}
```
### *Exercicio 5*
```kotlin
fun main() {
    val valorOriginal = readln().toDouble()
    val mesesAtraso = readln().toDouble()
    val taxaJuros = readln().toDouble()
    //  valor = valor_original * (1 + (taxa_juros / 100) * meses_atraso)
    val valorFinal = valorOriginal * (1.0 + (taxaJuros / 100.0) * mesesAtraso)
    println(valorFinal)
}

```
### *Exercicio 6*
```kotlin
fun main() {
    var a = readln().toInt()
    var b = readln().toInt()
    var c = b
     b = a
     a = c
    println(a)
    println(b)
}

```
### *Exercicio 7*
```kotlin
fun main() {
    var a = readln().toInt()
    var b = readln().toInt()
    var c = readln().toInt()
    var d = readln().toInt()
    
    println("Adições: $a+$b = ${a + b} $a+$c = ${a + c} $a+$d = ${a + d} $b+$c = ${b + c} $b+$d = ${b + d} $c+$d = ${c + d}")
    println("Mutiplicações: $a*$b = ${a * b} $a*$c = ${a * c} $a*$d = ${a * d} $b*$c = ${b * c} $b*$d = ${b * d} $c*$d = ${c * d}")

}
```
### *Exercicio 8*
```kotlin
fun main() {
    var comprimento = readln().toDouble()
    var largura = readln().toDouble()
    var altura = readln().toDouble()
    
    var volume = comprimento * largura * altura
    
    println(volume + " cm")
    // volume = comprimento * largura * altura
}
```
### *Exercicio 9*
```kotlin
import kotlin.math.pow

fun main() {
    var numero = readln().toDouble()
    var elevacao = readln().toDouble()
    var numeroElevado = numero.pow(elevacao)
    // quadrado = num * num
    println(numeroElevado)
}
```
### *Exercicio 10*
```kotlin
fun main() {
    var numero1 = readln().toDouble()
    var numero2 = readln().toDouble()
    
    println(numero1 - numero2)
    
    // diferenca = num1 - num2
}

```
### *Exercicio 11*
```kotlin
fun main() {
    var valorDolar = readln().toDouble()
    var cotacaoDolar = readln().toDouble()
    
    var valorReal = valorDolar * cotacaoDolar
    
    println(valorReal)
    
    // valor_em_real = valor_em_dolar * cotacao_do_dolar
}
```
### *Exercicio 12*
```kotlin
fun main() {
    var valorReal = readln().toDouble()
    var cotacaoDolar = readln().toDouble()
    
    var valorDolar = valorReal / cotacaoDolar
    
    println(valorDolar)
    
    // valor_em_dolar = valor_em_real / cotacao_do_dolar
}
```
### *Exercicio 13*
```kotlin
import kotlin.math.pow

fun main() {
    var n1 = readln().toDouble()
    var n2 = readln().toDouble()
    var n3 = readln().toDouble()
    
    // soma_quadrados = (num1 * num1) + (num2 * num2) + (num3 * num3)
    
    var somaQuadrados = n1.pow(2) + n2.pow(2) + n3.pow(2)
    
    println("$somaQuadrados ($n1² + $n2² + $n3² = ${n1.pow(2)} + ${n2.pow(2)} + ${n3.pow(2)}= $somaQuadrados)")
}

```
### *Exercicio 14*
```kotlin
import kotlin.math.pow

fun main() {
    var n1 = readln().toDouble()
    var n2 = readln().toDouble()
    var n3 = readln().toDouble()
    
    var somaQuadrados = (n1 + n2 + n3).pow(2)
    
    println("$somaQuadrados ($n1 + $n2 + $n3) = ${n1 + n2 + n3} = $somaQuadrados)")
}

```
### *Exercicio 15*
```kotlin
import kotlin.math.pow

fun main() {
    var n1 = readln().toDouble()
    var n2 = readln().toDouble()
    var n3 = readln().toDouble()
    var n4 = readln().toDouble()

    var som1 = n1 * n3
    var som2 = n2 + n4
    
    println("Produto: $n1 * $n3 = $som1")
    println("Soma: $n2 + $n4 = $som2")
}

```
### *Exercicio 16*
```kotlin
fun main() {
    var salario = readln().toDouble()
    var aumentoPorcentagem = readln().toDouble()
    var aumento = salario * (aumentoPorcentagem / 100)
    var novoSalario =  salario + aumento
    
    // aumento = salario * (aumento_porcentagem / 100)
    // novo_salario = salario + aumento
    
    println("Novo salario: $novoSalario aumento concedido = $aumento")
}
```
### *Exercicio 17*
```kotlin
import kotlin.math.pow

fun main() {
    val pi = 3.14159
    var raio = readln().toDouble()
    var area = pi * raio.pow(2)
    //area = 3.14159 * raio * raio
    println(area)
}
```
### *Exercicio 18*
```kotlin
fun main() {
    var votos_candidato1 = readln().toDouble()
    var votos_candidato2 = readln().toDouble()
    var votos_candidato3 = readln().toDouble()
    var votos_nulos = readln().toDouble()
    var votos_branco = readln().toDouble()
    
    var total_eleitores = votos_candidato1 + votos_candidato2 + votos_candidato3 + votos_nulos + votos_branco
    var percentual_candidato1 = (votos_candidato1 / total_eleitores) * 100
    var percentual_candidato2 = (votos_candidato2 / total_eleitores) * 100
    var percentual_candidato3 = (votos_candidato3 / total_eleitores) * 100
    var percentual_nulos = (votos_nulos / total_eleitores) * 100
    var percentual_branco = (votos_branco / total_eleitores) * 100
    
    println("total_eleitores = $total_eleitores")    
    println("percentual_candidato1 = $percentual_candidato1")
    println("percentual_candidato2 = $percentual_candidato2") 
    println("percentual_candidato3 = $percentual_candidato3")  
    println("percentual_nulos = $percentual_nulos")    
    println("percentual_branco = $percentual_branco")    
}
```
### *Exercicio 19*
```kotlin
fun main() {
   var val1 = readln().toDouble()
   var val2 = readln().toDouble()
   var adi = val1 + val2
   var sub = val1 - val2
   var mul = val1 * val2
   var div = val1 / val2
   
   println("Adição: $val1 + $val2 = $adi")
   println("Subtração: $val1 - $val2 = $sub")
   println("Mutiplicação: $val1 * $val2 = $mul")
   println("Divisão: $val1 / $val2 = $div")
   
    //adicao = valor1 + valor2
    //subtracao = valor1 - valor2
    //multiplicacao = valor1 * valor2
    //divisao = valor1 / valor2
}
```
### *Exercicio 20*
```kotlin
fun main() {
    var distancia = readln().toDouble()
    var tempo = readln().toDouble()
    
    var velocidade = distancia / tempo / 3.6
    
    println("Velocidade = $velocidade m/s")
}
```
### *Exercicio* 21
```kotlin
import kotlin.math.pow

fun main() {
    var base = readln().toDouble()
    var expoente = readln().toDouble()
    
    var potencia = base.pow(expoente)
    
    println(potencia)
}
```
### *Exercicio 22*
```kotlin
import kotlin.math.pow

fun main() {
    var raio = readln().toDouble()
    val pi = 3.1459
    var volume = (4/3) * pi * raio.pow(3)
    
    println(volume)
}
```
### *Exercicio 23*
```kotlin
fun main() {
    var medida_pes = readln().toDouble()
    var medida_metros = medida_pes * 0.3048
    
    println(medida_metros)
}
```
### *Exercicio 24*
```kotlin
import kotlin.math.pow

fun main() {
    var base = readln().toDouble()
    var indice = readln().toDouble()
    
    var raiz = base.pow(1/indice)
    
    println(raiz)
}
```
### *Exercicio 25*
```kotlin
fun main() {
    var num = readln().toInt()
    var sucessor = num + 1
    var antecessor = num - 1

    println("Sucessor = $sucessor. Antecessor = $antecessor")
}
```
### *Exercicio 26*
```kotlin
import kotlin.math.pow

fun main() {
    var num1 = readln().toDouble()
    var num2 = readln().toDouble()
    var resultado_divisao = num1 / num2
    var resultado_quadrado = resultado_divisao.pow(2)
    
    println(resultado_quadrado)
}
```

## ***Estrutura de Decisão***

### *Exercicio 27*
```kotlin
fun main() {
    var n1 = readln().toInt()
    var n2 = readln().toInt()
    var diferenca = n1 - n2
    if (n1 > n2){
        println(diferenca)
    } else {
        diferenca = n2 - n1
        println(diferenca)
    }
}
```
### *Exercicio 28*
```kotlin
fun main() {
    var n1 = readln().toInt()
    if (n1 > 0){
        println("Positivo")
    }else if(n1 == 0){
        println("Neutro")
    }else{
        println("Negativo")
    }
}
```
### *Exercicio 29*
```kotlin
fun main() {
    var nota1 = readln().toDouble()
    var nota2 = readln().toDouble()
    var nota3 = readln().toDouble()
    var nota4 = readln().toDouble()
    val media = (nota1 + nota2 + nota3 + nota4) / 4
    if(media >= 5){
        println("Média: $media Aprovado")
    } else {
        println("Média: $media Reprovado")
    }
}
```
### *Exercicio 30*
```kotlin
fun main() {
    var nota1 = readln().toDouble()
    var nota2 = readln().toDouble()
    var nota3 = readln().toDouble()
    var nota4 = readln().toDouble()
    val media = (nota1 + nota2 + nota3 + nota4) / 4
    if(media > 7){
        println("Média: $media Aprovado")
    } else if(media >= 5) {
        println("Média: $media Exame")
    } else {
        println("Média: $media Reprovado")
    }
}
```
### *Exercicio 31*
```kotlin
import kotlin.math.pow
import kotlin.math.sqrt

fun main() {
    var a = readln().toDouble()
    var b = readln().toDouble()
    var c = readln().toDouble()
    val delta = b.pow(2) - 4 * a * c
    if (delta >= 0){
        val x1 = (sqrt(delta) - b) / (2 * a)
        val x2 = (sqrt(delta) + b) / (2 * a)
        println("x1 = $x1, x2 = $x2")
    } else {
        println("Não existem raizes reais")
    }
}
```
### *Exercicio 32*
```kotlin
fun main() {
    var n1 = readln().toInt()
    var n2 = readln().toInt()
    var n3 = readln().toInt()
    var temp = n1
    if (n1 > n2){
        n1 = n2
        n2 = temp
    } else if(n1 > n3){
        n1 = n3
        n3 = temp
    } else if (n2 > n3){
        temp = n2
        n2 = n3
        n3 = temp
    }
    println("$n1, $n2, $n3")
}
```
### *Exercicio 33*
```kotlin
fun main() {
    var n1 = readln().toInt()
    var n2 = readln().toInt()
    var n3 = readln().toInt()
    var n4 = readln().toInt()
    if(n1 % 2 == 0 && n1 % 3 == 0){
        println(n1)   
    }
    if(n2 % 2 == 0 && n2 % 3 == 0){
        println(n2)
    }
    if(n3 % 2 == 0 && n3 % 3 == 0){
        println(n3)
    }
    if(n4 % 2 == 0 && n4 % 3 == 0){
        println(n4)
    }
}

```
### *Exercicio 34*
```kotlin
fun main() {
    var n1 = readln().toInt()
    var n2 = readln().toInt()
    var n3 = readln().toInt()
    var n4 = readln().toInt()
    if(n1 % 2 == 0 || n1 % 3 == 0){
        println(n1)   
    }
    if(n2 % 2 == 0 || n2 % 3 == 0){
        println(n2)
    }
    if(n3 % 2 == 0 || n3 % 3 == 0){
        println(n3)
    }
    if(n4 % 2 == 0 || n4 % 3 == 0){
        println(n4)
    }
    
}
```
### *Exercicio 35*
```kotlin
fun main() {
    var n1 = readln().toInt()
    var n2 = readln().toInt()
    var n3 = readln().toInt()
    var n4 = readln().toInt()
    var n5 = readln().toInt()
    
    var maiorValor = n1
    var menorValor = n1
    if (n2 > maiorValor){
        maiorValor = n2
    }
    if (n2 < menorValor){
        menorValor = n2
    }
    if (n3 > maiorValor){
        maiorValor = n3
    }
    if (n3 < menorValor){
        menorValor = n3
    }
    if (n4 > maiorValor){
        maiorValor = n4
    }
    if (n4 < menorValor){
        menorValor = n4
    }
    if (n5 > maiorValor){
        maiorValor = n5
    }
    if (n5 < menorValor){
        menorValor = n5
    }
    println("O maior numero é $maiorValor e o menor é $menorValor")
}

```
### *Exercicio 36*
```kotlin
fun main() {
    var n1 = readln().toInt()
    if (n1 % 2 == 0){
        println("Par")
    } else {
        println("Împar")
    }
}
```
### *Exercicio 37*
```kotlin
fun main() {
    var n1 = readln().toInt()
    if (n1 > 0 && n1 < 10){
        println("Valor está na faixa permitida")
    } else {
        println("Valor não está na faixa permitida")
    }
}
```
### *Exercicio 38*
```kotlin
fun main() {
    var n1 = readln().toInt()
    if (n1 <= 3){
        println(n1)
    } else {
        println("Nenhum valor apresentado")
    }
}
```
### *Exercicio 39*
```kotlin
fun main() {
    var n1 = readln().toInt()
    if (n1 % 3 == 0 && n1 % 5 == 0){
        println(n1)
    } else {
        println("Nenhum valor apresentado")
    }
}
```
### *Exercicio 40*
```kotlin
fun main() {
    var n1 = readln().toInt()
    var n2 = readln().toInt()
    var n3 = readln().toInt()
    if (n1 + n2 + n3 > 100){
        println("A soma de $n1, $2 e $n1 é igual a ${n1 + n2 + n3}, que é maior que 100.")
    } else {
        println("Nenhum valor apresentado")
    }
}
```
### *Exercicio 41*
```kotlin
fun main() {
    var n1 = readln().toInt()
    n1 *= 2
    if (n1 > 30){
        println(n1)    
    } else {
        println("Nenhum valor apresentado")
    }
}
```
## ***Estrutura de Repetição***

### *Exercicio 42*
```kotlin
import kotlin.math.pow

fun main() {
    var num = readln().toDouble()
    var quadrado = num.pow(2)
    var resultado_quadrados = num
    if(num > 14 && num < 201){
        resultado_quadrados = quadrado
        println(resultado_quadrados)
    } else {
        println("Fora da faixa")
    }
}
```
### *Exercicio 43*
```kotlin
fun main() {
    var num = readln().toInt()
    var multiplicador = 1
    var produto = num
    while(multiplicador < 11){
        produto = num * multiplicador
        println("$num x $multiplicador = $produto")
        multiplicador++
    }
}
```
### *Exercicio 44*
```kotlin
fun main() {
    var soma = 0
    var contador = 1
    while(contador < 101){
        println("$contador + $soma = ${contador + soma}")
        soma += contador
        contador++
    }
    println(soma)
}
```
### *Exercicio 45*
```kotlin
fun main() {
    var somaPares = 0
    for(nums in 2..500){
    if (nums % 2 != 0){
        continue
    } else {
        println("$somaPares + $nums = ${somaPares + nums}")
        somaPares += nums
    }
    }
}
```
### *Exercicio 46*
```kotlin
fun main() {
    var numero = 1
    while(numero <= 199){
        println(numero)
        numero +=2
    }
}
```
### *Exercicio 47*
```kotlin
fun main() {
    for(nums in 4..196 step 4){
        println(nums)    
    }
}
```
### *Exercicio 48*
```kotlin
import kotlin.math.pow

fun main() {
    var expoente = 0
    while(expoente <= 15){
        var potencia = 3.0.pow(expoente)
        println("3^$expoente = $potencia")
        expoente++
    }
}
```
### *Exercicio 49*
```kotlin
fun main() {
    var base = readln().toDouble()
    var expoente = readln().toInt()
    var potencia = base
    for(i in 1..expoente){
        potencia *= base
        println("$base elevado a $expoente = $potencia")
    }
}
```
### *Exercicio 50*
```kotlin
fun main() {
    var termo1 = 1
    var termo2 = 1
    println(termo1)
    println(termo2)
    var i = 3
    while(i <= 30){
        var proximoTermo = termo1 + termo2
        println(proximoTermo)
        termo1 = termo2
        termo2 = proximoTermo
        i++
    }
}
```
### *Exercicio 51*
```kotlin
fun main() {
    for (grauCelsius in 10..100 step 10){
        var grauFahrenheit = (grauCelsius * 9/5) + 32
        println("$grauCelsius °C = $grauFahrenheit °F")
    }
}
```
### *Exercicio 52*
```kotlin
import kotlin.math.pow

fun main() {
    var totalGraos = 0.0
    var quadro = 1
    while(quadro <= 64){
        var graosNoQuadro = 2.0.pow(quadro - 1)
        totalGraos += graosNoQuadro
        println("Total de grãos no tabuleiro é $totalGraos na casa $quadro")
        quadro++
    }
}
```
### *Exercicio 53*
```kotlin
fun main() {
    var somatorio = 0
    for(valor in 1..3){
        var fatorial = 1
        for(nums in 1..valor){
            fatorial += nums
            somatorio += fatorial
        }
    }
    println("Somatorio da fatorial de cada valor lido é $somatorio")
}
```
### *Exercicio 54*
```kotlin
fun main() {
    var somatorio = 0.0
    var contador = 0
    while(contador < 7){
        var valor = readln().toDouble()
        somatorio += valor
        contador++
    }
    var media = somatorio / contador
    println("Somatoio: $somatorio, Media: $media")
}
