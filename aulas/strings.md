# Introdução

O conceito de "string" é bastante simples. Uma string é uma sequência de carateres. 

Em Python as strings são imutáveis. 

Exercício: O que é um objeto imutável?


# Slice

Podemos cortar uma "fatia" de uma string utilizando a notação [a:b:c]. 

- a: posição de início da "fatia";
- b: posição final da "fatia";
- c: passo entre o início e o final.

O passo (stride) pode ser negativo, retornando os itens em "reverse".

```
>>> s = 'bicycle'
>>> s[::3]
'bye'
>>> s[::-1]
'elcycib'
>>> s[::-2]
'eccb'
```

## replace

O método ```replace()``` substitui uma frase por outra frase.

```
string.replace(valor_antigo, novo_valor, conta)
```

- valor_antigo - Obrigatório. A string a ser procurada.
- novo_valor - Obrigatório. A string que irá substituir
- count - O número de vezes a substituir a string. Se não for especificado, todas as ocorrências irão ser substituídas.

## Grupos

- Grupo 1
    - Bernardo
    - Veiga
- Grupo 2
    - Hugo
    - Alves
- Grupo 3
    - Sousa
    - Beatriz
- Grupo 4
    - Afonso
    - Júnior
- Grupo 5
    - Cristiano
    - Filipe
- Grupo 6
    - Davi
    - Daniel

## Trabalho

- capitalize()	Converts the first character to upper case
- casefold()	Converts string into lower case
- center()	Returns a centered string
- count()	Returns the number of times a specified value occurs in a string
- encode()	Returns an encoded version of the string
- endswith()	Returns true if the string ends with the specified value
- expandtabs()	Sets the tab size of the string
- find()	Searches the string for a specified value and returns the position of where it was found
- format()	Formats specified values in a string
- format_map()	Formats specified values in a string
- index()	Searches the string for a specified value and returns the position of where it was found
- isalnum()	Returns True if all characters in the string are alphanumeric
- isalpha()	Returns True if all characters in the string are in the alphabet
- isascii()	Returns True if all characters in the string are ascii characters
- isdecimal()	Returns True if all characters in the string are decimals
- isdigit()	Returns True if all characters in the string are digits
- isidentifier()	Returns True if the string is an identifier
- islower()	Returns True if all characters in the string are lower case
- isnumeric()	Returns True if all characters in the string are numeric
- isprintable()	Returns True if all characters in the string are printable
- isspace()	Returns True if all characters in the string are whitespaces
- istitle()	Returns True if the string follows the rules of a title
- isupper()	Returns True if all characters in the string are upper case
- join()	Converts the elements of an iterable into a string
- ljust()	Returns a left justified version of the string
- lower()	Converts a string into lower case
- lstrip()	Returns a left trim version of the string
- maketrans()	Returns a translation table to be used in translations
- partition()	Returns a tuple where the string is parted into three parts
- replace()	Returns a string where a specified value is replaced with a specified value
- rfind()	Searches the string for a specified value and returns the last position of where it was found
- rindex()	Searches the string for a specified value and returns the last position of where it was found
- rjust()	Returns a right justified version of the string
- rpartition()	Returns a tuple where the string is parted into three parts
- rsplit()	Splits the string at the specified separator, and returns a list
- rstrip()	Returns a right trim version of the string
- split()	Splits the string at the specified separator, and returns a list
- splitlines()	Splits the string at line breaks and returns a list
- startswith()	Returns true if the string starts with the specified value
- strip()	Returns a trimmed version of the string
- swapcase()	Swaps cases, lower case becomes upper case and vice versa
- title()	Converts the first character of each word to upper case
- translate()	Returns a translated string
- upper()	Converts a string into upper case
- zfill()	Fills the string with a specified number of 0 values at the beginning


## Avançado 

### Carateres

In 2021, the best definition of “character” we have is a Unicode character. Accordingly, the items we get out of a Python 3 str are Unicode characters, just like the items of a unicode object in Python 2—and not the raw bytes we got from a Python 2 str.

.zfill() 
print("""a funçao .zfill() vai adicionar a quantidade de 0 para concluir um numero de casas o mesmo funciona com palavras""")
numero = "30"
print(numero.zfill(3))
texto = "texto"
print(texto.zfill(9))

.upper()
print("""a funçao upper vai deixar a frase em Caps Lock ou seja:""")
texto = "arroz é bom"
print(texto.upper())
texto = "isto nao se  faz 02"
print(texto.upper())
texto = "Sim eu nao sei"
print(texto.upper())

.translate()
print("""basicamnte o translate vai retornar uma especie de traduçao""")
a= {9: 2}
texto = "caneta azul, azul caneta"
print(texto.translate(a))
b= {3: 6}
texto = "isto es em altas"
print(texto.translate(b))
c= {29: 9}
texto = "vamos passear "
print(texto.translate(c))

.title()
print("""basicamento o title() vai tranformar todas a primeira letra de cada palavra em upper case ou seja:""")
texto = "eu nao sei ler"
print(texto.title())
texto = "vamos brincar"
print(texto.title())
texto = "eu gosto de jogar"
print(texto.title())

.swapcase()
print("""basicamnete o swapcase() faz com que as letras maiusculas se tornem minusculas e virce versa""")
texto = "EEEEE NNNN uus sss"
print(texto.swapcase())
texto = "Milimetro é diferente"
print(texto.swapcase())
texto = "Eu Nao Sei"
print(texto.swapcase())

.strip
print("""basicamente o strip() vai fazer com que a frase naoo contem o numero de espeços desnecessarios
ou seja:""")
texto = "banana"
print("minha fruta favorita é",texto.strip())
texto = "verde"
print("minha cor favorita é",texto.strip())
texto = "maça"
print("minha fruta favorita é",texto.strip())


.startswith
print("""basicamente o startswith vai retornar se é True or False caso a palavra inserida esta no inicio da frase
ou seja:""")

txt = "eu gosto do verao"
print(txt.startswith('eu'))
print(txt.startswith('verao'))

.sliplines
print("""basicamente a funçao "splitlines" vai receber uma string e tranformando em lista
ou seja:""")

txt = "eu nao sei"
print(txt.splitlines())
txt = "eu nao s3i \n a"
print(txt.splitlines())
txt = "aA \n nnnnnn \n ddddd "
print(txt.splitlines())
