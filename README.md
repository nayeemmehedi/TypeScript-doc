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






 
