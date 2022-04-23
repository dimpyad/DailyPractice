## Learning Goal
Single responsibility principle

### Problem Statement
1. Identify the problems in the below code
2. Improve the code by applying single responsibility principle. You can add new interface/classes if required.
```
public class Animal{
private Integer id;
private String name;
private Connection con = null;

public void saveAnimal(){
// Save animal object to database
}

public Animal getAnimal(int id)
{
  // get animal from database based on id
  Animal animal = null;
  //some code
  return animal;
}

public boolan validate()
{
return id!=null && id>0;
}

}
```
