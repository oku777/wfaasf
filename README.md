import matplotlib.pyplot as plt

# Datos para 2021
data_2021 = {
    "Proyecto": ["Bogotá Solidaria", "Educación Inicial", "Desarrollo Social"],
    "Meta": [25000, 10, 18000]
}

# Datos para 2021-2024
data_2021_2024 = {
    "Proyecto": ["Bogotá Solidaria", "Educación Inicial", "Desarrollo Social"],
    "Meta": [27000, 14, 20000]
}

# Datos para 2024
data_2024 = {
    "Proyecto": ["Bogotá Solidaria", "Educación Inicial", "Desarrollo Social"],
    "Meta": [28000, 18, 22000]
}

# Crear subplots
fig, axes = plt.subplots(1, 3, figsize=(18, 6), sharey=True)

# Gráfica para 2021
axes[0].bar(data_2021['Proyecto'], data_2021['Meta'], color='skyblue')
axes[0].set_title('Meta Proyecto 2021')
axes[0].set_xlabel('Proyectos')
axes[0].set_ylabel('Meta')

# Gráfica para 2021-2024
axes[1].bar(data_2021_2024['Proyecto'], data_2021_2024['Meta'], color='teal')
axes[1].set_title('Meta Proyecto 2021-2024')
axes[1].set_xlabel('Proyectos')

# Gráfica para 2024
axes[2].bar(data_2024['Proyecto'], data_2024['Meta'], color='lightgreen')
axes[2].set_title('Meta Proyecto 2024')
axes[2].set_xlabel('Proyectos')

plt.tight_layout()
plt.show()
