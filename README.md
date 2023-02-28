# Tarea1Parcial2
Herencia Multiple:
La herencia múltiple se encuentra en aquellos casos en los que una clase se hereda (se deriva) de mas de una clase.
Java no soporta la herencia multiple ya que una clase concreta solo puede tener una clase padre.
Investigacion:
- Conflictos de nombres y ambigüedad. Cuando los compiladores de los lenguajes de programación que soportan este tipo de superclases 
  de sucesión múltiple contienen métodos con el mismo nombre, a veces no pueden determinar a qué miembro o método acceder o invocar.
- Además, un programador puede involuntariamente introducir un conflicto de nombres añadiendo un nuevo método a una superclase.

class Person{
  - String name;
  - LocalDate birthday;
 
 
  + getName(): String;
  + setName(String name);
 
  + getBirthday(): LocalDate;
  + setBirthday(LocalDate birthday);
}

class Employee extends Person {
  - String rpe;
 
  + getRpe(): String;
  + setRpe(String rpe);
}

class Student extends Person {
 
  - String code;
 
  + getCode(): String;
  + setCode(String code);
 
}

class Professor extends Employee  {

}


class Concierge extends Employee{


}

class AdministrativePerson  extends Employee{
}


class ScholarshipHolder  extends Employee {
  - String code;
 
  + getCode(): String;
  + setCode(String code);
}

