# Tarea3

Para esta tarea se eligen confeccionar una tabla nutricional de alimentos que tenga los siguientes elementos:
- Nombre
- Kcal
- HC (hidratos de carbono)
- Prot (proteínas)
- Grasas
- Categoría
- Tipo

Se usa como referencia la tabla de http://www.portalfitness.com/nutricion/tabla_calorias_b.htm para extraer todos los alimentos que aparecen en el documento .xml, pese a que tiene una información desacertada en muchos y una categorización de varios grupos de alimentos bastante mal estructurada. Se han readaptado algunos nombres sudamericanos al castellano.

Como no me terminaba de quedar claro la cantidad de nodos solicitados puse 27 alimentos. Cada uno con sus respectivos elementos. No se usaron atributos en primera instancia siguiendo las recomendaciones de w3school y se optó por agregar elementos adicionales como categoría y la subcategoría tipo para definir los alimentos.

Como quedaba muy simple el documento y el DTD, finalmente me decanté por incluir el atributo código como ID para hacer único cada uno de éstos. 

Tras seguir hacendo comprobaciones con el validador de https://www.xmlvalidation.com/ no se consigue que reconozca correctamente el documento .dtd. Si pongo éste dentro del .xml lo valida correctamente, al igual que otros validadores con los que hice pruebas ( https://codebeautify.org/xmlvalidator# y https://www.truugo.com/xml_validator/ ) pero que lamentablemente no permiten usar un dtd externo. Como alternativa, subo un documento adicional llamado tablanutricional(xml+dtd).xml para que se pueda comprobar facilmente.
