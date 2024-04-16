# Gestion-de-productos
Quiero crear una funcion que me permita modificar el precio , cantidad , nombre de mi lista y se guarde en los archivos json actualizado .Me pueden ayudar porfa? 
def actualizar_listbox():
    lista_productos_lb.delete(0, tk.END)  # Borra todos los elementos del Listbox
    for producto in lista_productos:
        nombre = producto["Nombre del Producto"]
        precio = producto["Precio"]
        cantidad = producto["Cantidad Stock"]
        lista_productos_lb.insert(tk.END, f"{nombre} - Precio: {precio} - Stock: {cantidad}")
