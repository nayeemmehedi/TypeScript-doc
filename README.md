## TypeScript doc
...................

 1. array :
..................


        a.let newArray:string[]  🍻
        b.let newArray: Array<string>
        c.let values: (string | number)[]
        d.let values: Array <string | number>


2. Tuples : fixed value
....................

       let ourTuples : [ name:string, age:number ]
       
       ourtuples = [name:"bangla",age:34]

3.Object :

     let car: { type: string, model: string, year: number }

3.a.Index Signatures : jkono key add krte prbo but number


    const nameAgeMap: { [index: string]: number } = {};

 4.Enum : unchangeable variables -> j value dbe object r moto paya jbe .

example:

     enum GenderEnum {
     female = "female",
     male = "male",
     other = "other",
   }
   
    interface IFormInput {
      firstName: string
      gender: GenderEnum
    }
   
    let value: IFormInput = {
      firstName: "ddd",
      gender: GenderEnum.female
    }

 5. Type Aliases


        type CarYear = number
        type CarType = string
        type CarModel = string
        type Car = {
          year: CarYear,
          type: CarType,
          model: CarModel
        }
6.Interfaces 

    interface Rectangle {
      height: number,
      width: number
    }
    
    const rectangle: Rectangle = {
      height: 20,
      width: 10
    };

 7.Generic : 

     function createPair<S, T>(v1: S, v2: T): [S, T] {
     return [v1, v2];
   }
      
    console.log(createPair<string, number>('hello', 42));





 
