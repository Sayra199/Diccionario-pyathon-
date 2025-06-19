cliente_dxn = {
    "nombre": "Ana",
    "país": "México",
    "productos_comprados": 3,
    "cliente_activo": True
}

# Actualización de datos
cliente_dxn["productos_comprados"] += 2
cliente_dxn["nivel"] = "Afiliado Oro"
del cliente_dxn["cliente_activo"]

print(cliente_dxn)