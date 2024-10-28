## Explicación Extraxt Subclase

Extract Subclass es un patrón de refactorización orientado a simplificar una clase al dividir parte de su 
funcionalidad en una subclase. Este patrón se usa generalmente cuando una clase realiza múltiples funciones
que podrían delegarse a una subclase, mejorando así la organización y facilitando el mantenimiento
del código.

## Ejemplo de Cuándo Usar Extract Subclass

Imagina una clase Empleado que maneja tanto tareas administrativas como de desarrollo de software. Si estas 
funciones son distintas y tienen reglas o métodos diferentes, podemos aplicar Extract Subclass para crear 
subclases específicas, como EmpleadoAdministrativo y Desarrollador. Esto hace que el código sea más fácil 
de leer y menos propenso a errores.

## Pasos para Aplicar Extract Subclass

1.- Identifica el conjunto de métodos y atributos específicos que representan una funcionalidad diferente dentro de la clase. \n
2.- Crea una subclase para agrupar esos métodos y atributos.\n
3.- Transfiere los métodos y atributos relevantes de la clase original a la nueva subclase.\n
4.- Ajusta las referencias en otras partes del código para utilizar la nueva subclase cuando corresponda.\n
5.- Prueba el código para asegurarte de que la funcionalidad no se vea afectada tras la refactorización.\n

## Beneficios de Extract Subclass

Claridad: La separación de responsabilidades hace que cada clase sea más clara y fácil de entender.
Mantenimiento: Cada clase está menos sobrecargada de métodos innecesarios y es más fácil de mantener.
Extensibilidad: Facilita la adición de nuevas funcionalidades específicas a cada subclase sin afectar a la clase principal.
