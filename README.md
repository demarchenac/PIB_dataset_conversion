# Conversion de los datos del PIB
Jupyter notebook desarrollado con el fin de convertir la fuente de datos del DANE y el Banco de la república para el PIB a precios constantes, en un formato horario y desagregado por departamentos.

## Dependencias
- [datetime](https://github.com/zopefoundation/DateTime)
- [matplotlib](https://matplotlib.org/)
- [numpy](https://numpy.org/)
- [pandas](https://pandas.pydata.org/)
- [seaborn](https://seaborn.pydata.org/)
- [scikit-learn](https://scikit-learn.org/stable/#)
- [xgboost](https://github.com/dmlc/xgboost)

## Fuentes de datos:
- DANE: **[PIB total por departamentos](https://www.dane.gov.co/index.php/estadisticas-por-tema/cuentas-nacionales/cuentas-nacionales-departamentales)**
- Banco de la república: Seleccionamos **[Todas las series de datos](https://www.banrep.gov.co/es/estadisticas/producto-interno-bruto-pib)** y se nos abrira una ventana nueva, en esta ventana exportamos los datos del gráfico de la pestaña del PIB en formato csv.

## Formato de la fuentes de datos (Proceso previo a la ejecucción del notebook).

Para el archivo del DANE, **anexo-{YYYY}-provisional-PIB-total-por-departamento.xlsx**, copiamos la tabla en la hoja **Cuadro 2**:

![image](https://user-images.githubusercontent.com/20970325/167273990-2c2c133c-a3ba-4d53-b70e-489f8ca19445.png)


En una nueva hoja la cual llamaremos **export**, y finalmente seleccinamos todas las celdas y cambiamos su formato a **General**:

![image](https://user-images.githubusercontent.com/20970325/167274236-1f197285-bd5b-41cc-97b4-0bdf4f764a45.png)

Para el archivo csv del Banco de la república, **Producto Interno Bruto_PIB_Grafica.csv**, solo nos encargamos de cambiar el formato de todas las celdas de este a **General**

*Es importante tomar en cuenta que los datos númericos han de quedar sin separadores de miles (,) y  solo con su unico separador decimal (.)*


## Instalar dependencias
Para instalar las dependencias simplemente ejecutaremos `pip3 install -r requirements.txt`, en el mismo directorio en el cual se encuentre el notebook.
