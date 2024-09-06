# tarea12
# Definimos una matriz 3D (Ciudades, Días de la semana, Semanas)
temperaturas = [
    # Ciudad 1
    [
        [20, 22, 21, 19, 23, 24, 25], # Semana 1
        [22, 23, 21, 20, 24, 26, 27], # Semana 2
    ],
    # Ciudad 2
    [
        [15, 17, 16, 14, 18, 19, 20], # Semana 1
        [16, 18, 17, 15, 19, 21, 22], # Semana 2
    ]
]

# Nombres de las ciudades
ciudades = ['Quito', 'Guayaquil']

# Inicializamos bucles anidados para iterar sobre ciudades y semanas
for ciudad_idx, ciudad in enumerate(temperaturas):
    print(f"Promedio de temperaturas para {ciudades[ciudad_idx]}:")
    
    # Iteramos sobre semanas
    for semana_idx, semana in enumerate(ciudad):
        # Calculamos el promedio de la semana
        promedio_semana = sum(semana) / len(semana)
        print(f"  Semana {semana_idx + 1}: {promedio_semana:.2f}°C")
