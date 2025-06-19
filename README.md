Client_DXN cliente_dxn = {
    "nombre": "Ana",
    "país": "México",
    "productos_comprados": 3,
    "nivel": "Afiliado Oro"
}

# Mostrar datos del cliente
print("Datos actuales del cliente:")
for clave, valor in cliente_dxn.items():
    print(f"{clave}: {valor}")

# Agregar nueva información
cliente_dxn["activo"] = True
cliente_dxn["email"] = "ana@email.com"

# Buscar una clave
busqueda = input("\n¿Qué dato deseas consultar? (ej: país, nivel, email): ")
valor = cliente_dxn.get(busqueda, "Dato no encontrado.")
print(f"\nResultado de búsqueda: {valor}")

# Actualizar productos comprados
cliente_dxn["productos_comprados"] += 2

# Mostrar resumen final
print("\nResumen actualizado:")
for clave, valor in cliente_dxn.items():
    print(f"{clave}: {valor}")