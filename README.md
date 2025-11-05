# Página escolar - Cálculo de média anual do aluno

print("=== Sistema de Notas Escolares ===")

# Lista para armazenar todas as notas
notas = []

# Coleta das 9 notas (3 por trimestre)
for i in range(1, 10):
    nota = float(input(f"Digite a nota {i}: "))
    notas.append(nota)

# Cálculo das médias trimestrais
media_1 = sum(notas[0:3]) / 3
media_2 = sum(notas[3:6]) / 3
media_3 = sum(notas[6:9]) / 3

# Soma total das médias trimestrais
soma_medias = media_1 + media_2 + media_3

# Exibe resultados
print("\n=== Resultados ===")
print(f"Média 1º trimestre: {media_1:.2f}")
print(f"Média 2º trimestre: {media_2:.2f}")
print(f"Média 3º trimestre: {media_3:.2f}")
print(f"Soma das médias: {soma_medias:.2f}")

# Verifica aprovação
if soma_medias >= 48:
    print("✅ Aluno APROVADO!")
else:
    print("❌ Aluno REPROVADO!")
