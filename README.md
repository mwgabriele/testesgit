## Python
readme de testes.

**Primeiro** `push`

### **Criando Arrays em Python**

Python não possui suporte integrado para arrays, mas oferece um objeto listado que pode ser usado de forma semelhante. No entanto, para arrays numéricos, Python fornece um módulo de array especializado que pode ser usado para criar arrays com elementos de um tipo específico.

### Lista em Python como um Array

```python
# Criando uma lista
my_list = [10, 20, 30, 40, 50]
print(my_list)

```

### Usando o Módulo de Array

```python
from array import array

# Criando um array de tipo inteiro
my_array = array('i', [10, 20, 30, 40, 50])
print(my_array)

```

### **Acessando Elementos do Array**

Elementos do array podem ser acessados usando seu índice. Os índices em arrays começam do 0, o que significa que o primeiro elemento do array é acessado por **`0`**, o segundo elemento por **`1`**, e assim por diante.

```python
# Acessando o primeiro elemento
print(my_list[0])  # Output: 10
print(my_array[0])  # Output: 10

```

### **Modificando Elementos do Array**

Elementos do array podem ser modificados acessando-os usando seu índice e, em seguida, atribuindo um novo valor.

```python
# Modificando o primeiro elemento
my_list[0] = 100
my_array[0] = 100

print(my_list)  # Output: [100, 20, 30, 40, 50]
print(my_array)  # Output: array('i', [100, 20, 30, 40, 50])
```

#### **Operações Básicas**

- **Comprimento**: **`len(my_list)`** ou **`len(my_array)`**
- **Adicionando Elementos**: Para listas, **`my_list.append(60)`**; para arrays, **`my_array.append(60)`**
- **Removendo Elementos**: Para listas, **`my_list.remove(30)`**; para arrays, **`my_array.remove(30)`**

#### 02 de maio de 2025

Comando `max` :

```python
# Mostrando o maior valor entre duas variáveis
largest_num = max(num1, num2)
```

---

```python
from pasta.arquivo import funcao
```

### Módulo e Pacote

Pacotes contêm módulos. Um diretório se torna um pacote quando contém o arquivo **init**.py, que também resulta na criação da pasta *pycache*

> from . import modulo
>
> O `.` significa que está contido naquele pacote, naquele diretório
>
> diretório.arquivo import funcao
>
> se colocar o arquivo no init torna público a função e não precisa chamar diretório.arquivo
>
> init é como o prefácio dos módulos dentro do meu pacote
>
> um módulo para o menu, um módulo para as minhas funções e o meu algoritmo principal que está fora de tudo.

```python
from .tratamento_excecoes import dividir_numeros, somar_numeros
```

---

```python
if __name__ = "__main__":
	menu_principal()
```

#### /n

A barra invertida ( **`\`**) tem um significado muito especial quando usada dentro de strings ‒ é chamada **de caractere de escape** .

A palavra *escape* deve ser entendida especificamente: significa que a série de caracteres na string escapa por um momento (um momento muito curto) para introduzir uma inclusão especial.

Em outras palavras, a barra invertida não significa nada em si, mas é apenas uma espécie de anúncio de que o próximo caractere depois da barra invertida também tem um significado diferente.

A letra **`n`**colocada depois da barra invertida vem da palavra *newline* .

Tanto a barra invertida quanto o *n* formam um símbolo especial chamado **caractere de nova linha**, que solicita ao console que inicie uma **nova linha de saída**.

> Um computador […] é desprovido de qualquer traço de inteligência. Pode-se dizer que é como um cachorro bem treinado: ele responde apenas a um conjunto predeterminado de comandos conhecidos.