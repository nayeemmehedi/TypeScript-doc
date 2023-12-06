## TYPESCRIPT DOCTYPE

type :

    type CarYear = number
    type Car = {
      year: CarYear,
      type: CarType,
      model: CarModel
    }
    
    const carYear: CarYear = 2001
    
    const car: Car = {
      year: carYear,
      type: carType,
      model: carModel
    };

    
Interfaces :

    interface Rectangle {
      height: number,
      width: number
    }
    
    const rectangle: Rectangle = {
      height: 20,
      width: 10
    };


Tupes :

A tuple is a typed array with a pre-defined length and types for each index.

    let ourTuple: [number, boolean, string];
  
    ourTuple = [5,false,'Coding God was mistaken'];

Enum :
    
    enum StatusCodes {
      NotFound = 404,
      Success = 200,
      Accepted = 202,
      BadRequest = 400
    }
    // logs 404
    console.log(StatusCodes.NotFound);


Generics :

1st example 

      function identity<T>(value: T): T {
      return value;
     }
    
    const result = identity<number>(123);


2nd example :  Passing Type Parameters Directly


       type ProgrammingLanguage = {
        name: string;
       };
    
    function identity<T>(value: T): T {
      return value;
    }
    
    const result = identity<ProgrammingLanguage>({ name: "TypeScript" });


3rd example : 


     interface MyInterface<T> {
        field: T;
      }
    
    const example1: MyInterface<number> = { field: 123 };
    const example2: MyInterface<string> = { field: "Hello, TypeScript!" };
    const example3: MyInterface<boolean> = { field: true };








