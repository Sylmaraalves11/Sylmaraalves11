# Exercício 01 – Verificador de Palíndromo
import unicodedata

def remover_acentos(texto):
    return ''.join(c for c in unicodedata.normalize('NFD', texto)
                   if unicodedata.category(c) != 'Mn')

def eh_palindromo(frase):
    frase = remover_acentos(frase.lower().replace(" ", "").replace(",", "").replace(".", ""))
    return frase == frase[::-1]

entrada = input("Digite uma palavra ou frase: ")
if eh_palindromo(entrada):
    print("É um palíndromo!")
else:
    print("Não é um palíndromo.")
