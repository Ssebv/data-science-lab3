## ANOVA

### REQUERIMIENTOS
- Se utilizo vscode con la extension de r y rmarkdown
- Archivo .rmd
- R - Notebook vscode

# Introducción

En este análisis, exploraremos el rendimiento estudiantil en dos escuelas portuguesas utilizando un conjunto de datos que contiene una variedad de características demográficas, sociales y relacionadas con la escuela. 

Nuestro objetivo principal es entender qué factores influyen en las calificaciones finales de los estudiantes.

## Variables de Interés

### Variable Dependiente (VD): Calificación Final (G3)

La variable de interés principal en nuestro análisis es la calificación final en el tercer período escolar, representada por la variable "G3". 

Esta variable es crucial, ya que refleja el rendimiento académico de los estudiantes al final del año escolar.

Como afectaran diferentes variables independientes a la calificación final de los estudiantes.

### Variables Independientes (VI)

1. **school**: La escuela a la que asisten los estudiantes ('GP' para Gabriel Pereira o 'MS' para Mousinho da Silveira).

2. **sex**: El género del estudiante ('F' para femenino o 'M' para masculino).

3. **age**: La edad del estudiante.

4. **address**: El tipo de dirección del estudiante ('U' para urbano o 'R' para rural).

5. **famsize**: El tamaño de la familia del estudiante ('LE3' para menos o igual a 3 o 'GT3' para más de 3).

6. **Pstatus**: El estado de convivencia de los padres ('T' para juntos o 'A' para separados).

7. **Medu**: La educación de la madre (en una escala de 0 a 4).

8. **Fedu**: La educación del padre (en una escala de 0 a 4).

9. **Mjob**: La ocupación de la madre.

10. **Fjob**: La ocupación del padre.

11. **reason**: La razón para elegir la escuela ('home' para cercanía a casa, 'reputation' para reputación, 'course' para preferencia de curso, 'other' para otras razones).

12. **guardian**: El tutor legal del estudiante.

13. **traveltime**: El tiempo de viaje desde casa a la escuela (en una escala de 1 a 4).

14. **studytime**: El tiempo semanal de estudio (en una escala de 1 a 4).

15. **failures**: El número de clases falladas (en una escala de 1 a 4).

16. **schoolsup**: Apoyo educativo extra de la escuela ('yes' o 'no').

17. **famsup**: Apoyo educativo extra de la familia ('yes' o 'no').

18. **paid**: Clases extra pagadas ('yes' o 'no').

19. **activities**: Participación en actividades extracurriculares ('yes' o 'no').

20. **nursery**: Asistencia a guardería infantil ('yes' o 'no').

21. **higher**: Aspiración de educación superior ('yes' o 'no').

22. **internet**: Acceso a Internet en casa ('yes' o 'no').

23. **romantic**: Relación romántica ('yes' o 'no').

24. **famrel**: Calidad de las relaciones familiares (en una escala de 1 a 5).

25. **freetime**: Tiempo libre después de la escuela (en una escala de 1 a 5).

26. **goout**: Frecuencia de salir con amigos (en una escala de 1 a 5).

27. **Dalc**: Consumo de alcohol en días laborables (en una escala de 1 a 5).

28. **Walc**: Consumo de alcohol en fines de semana (en una escala de 1 a 5).

29. **health**: Estado de salud (en una escala de 1 a 5).

30. **absences**: Cantidad de ausencias escolares.

31. **G1**: Calificación en el primer período.

32. **G2**: Calificación en el segundo período.

# Modelado y Objetivos
Este conjunto de datos se ha utilizado para tareas de clasificación binaria/de cinco niveles y tareas de regresión. Un aspecto importante es que las calificaciones G3 tienen una fuerte correlación con las calificaciones G2 y G1. Esto se debe a que G3 es la calificación final del último año, mientras que G1 y G2 son calificaciones de los primeros dos períodos. Esta relación es esencial para predecir el rendimiento estudiantil.

# Uso del Conjunto de Datos
Este conjunto de datos es valioso para llevar a cabo análisis de datos, modelado predictivo y evaluación del rendimiento académico de los estudiantes. Puede ser utilizado en investigaciones educativas y análisis de factores que afectan el éxito académico de los estudiantes en la educación secundaria.

Explica lo que los resultados del test significan en el contexto de tu problema.
¿Son estadísticamente significativos?
¿Qué implicaciones tienen?

# como la prueba de Breusch-Pagan o la prueba de White.
El test estadistico de Breusch-Pagan es un análisis de regresión para evaluar la presencia de heterocedasticidad en los residuos de un modelo. La heterocedasticidad se refiere a la situación en la que la varianza de los errores (residuos) no es constante en todos los niveles de las variables predictoras, lo que viola uno de los supuestos clave de la regresión lineal. Se utiliza para determinar si la varianza de los residuos está relacionada con una o más variables independientes del modelo. La presencia de heterocedasticidad puede afectar la eficiencia y validez de las estimaciones de los coeficientes de regresión, los intervalos de confianza y las pruebas de hipótesis.

# Anova
Es una tecnica estadistica utilizada para comparar las variacion de diferentes muestras, poblaciones o grupos y determinar si existen diferencias significativas entre ellas.
