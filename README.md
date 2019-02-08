# Tarea3

Para esta tarea se eligen confeccionar una tabla nutricional de alimentos que tenga los siguientes elementos:
- Nombre
- Kcal
- HC (hidratos de carbono)
- Prot (proteínas)
- Grasas
- Categoría
- Tipo

Se usa como referencia la tabla de *http://www.portalfitness.com/nutricion/tabla_calorias_b.htm* para extraer todos los alimentos que aparecen en el documento .xml, pese a que tiene una información desacertada en muchos y una categorización de varios grupos de alimentos bastante mal estructurada. Se han readaptado algunos nombres sudamericanos al castellano.

#### 06/02/2019

Como no me terminaba de quedar claro la cantidad de nodos solicitados puse 27 alimentos. Cada uno con sus respectivos elementos. No se usaron atributos en primera instancia siguiendo las recomendaciones de w3school y se optó por agregar elementos adicionales como categoría y la subcategoría tipo para definir los alimentos.

Como quedaba muy simple el documento y el DTD, finalmente me decanté por incluir el atributo código como ID para hacer único cada uno de éstos. La ID hace referencia a la categoría (primer dígito), tipo (segundo dígito) y el alimento de esa clase (dos últimos dígitos). Se escoge esta opción para tratar de hacer el documento escalable en el tiempo, con vista de ser gestionado como una base de datos.

+ #### 07/02/2018 Obsoleto

+ Tras seguir hacendo comprobaciones con el validador de https://www.xmlvalidation.com/ no se consigue que reconozca correctamente el documento .dtd. Si pongo éste dentro del .xml lo valida correctamente, al igual que otros validadores con los que hice pruebas ( https://codebeautify.org/xmlvalidator# y https://www.truugo.com/xml_validator/ ) pero que lamentablemente no permiten usar un dtd externo. Como alternativa, subo un documento adicional llamado tablanutricional(xml+dtd).xml para que se pueda comprobar facilmente.

_No se llega a subir el documento, se corrigen los errores tras las consultas en foro.


### 08/02/2018 Actualización final:

Entender y aplicar XSD ha sido bastante más complicado que xml y DTD, ya que ofrece muchas funcionalidades a cambio de un lenguaje mas complejo de enteder. Se hace empleo del programa Oxygen que se menciona en el temario de la IOC y se migra el esquema DTD a Schema, facilitando bastante confeccionar su estructura. Estaba tratando de conseguir que los tipos estuvieran restringidos a la categoría, pero finalmente no lo conseguí, posiblemente porque trataba de acomodarlo como una base de datos pero aquí posiblemente no sea posible, y/o huviera que hacer uso de atributos para estructurarlos.

      Aun así, se completan con éxito todos los puntos solicitados en la tarea Saludos.
