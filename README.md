# TypeScript-doc basic to advance

https://www.typescripttutorial.net/typescript-tutorial/typescript-type-aliases/
https://devsonket.com/typescript

##### basic

           function nameFunc(name: string,value : number){

		    console.log(name,value)

            }


	     nameFunc("string",3)





#### #event (form) type  =>  React.FormEvent<EventTarget>
	
	
	Example 
	
	
	  function SubmitValue(event:React.FormEvent<EventTarget>){
             event.preventDefault()
             console.log("hello");
      
           }

### 1st example :  Object Types


		

                  function Cool ( pt: { x: number; y: number })  {

                         console.log(   pt.x   )
                         console.log(   pt.y   )

                    }

                   printCoord({ x: 3, y: 7 })


### 2nd Example :  Optional Properties


         function Cool(obj: { first: string; last?: string }) {

               //something
           
          }

          Cool  ({ first: "Bob" })

           Cool  ({ first: "Alice", last: "Alisson" })


### 3rd example :  Union Types

        function printId(id: number | string) {
               console.log("Your ID is: " + id);
          }


### 4th example :  Type Aliases


            type Point = {

            x: number;
            y: number;

            }
 

            function cool (pt: Point) {

            console.log(  pt.x )
            console.log(  pt.y  )

            }
 
            cool ({ x: 100, y: 100 })


### 5th example :  Interfaces

            interface Point {
            x: number;
            y: number;
            }
            
            function cool (pt: Point) {

            console.log(  pt.x )
            console.log(  pt.y  )

            }
            
            cool ({ x: 100, y: 100 })







### 6th example :   Interfaces vs Type Aliases

Interfaces:

            interface Animal {
            name: string
            }

            interface Bear extends Animal {
            honey: boolean
            }

            const bear = getBear() 
            bear.name
            bear.honey


Type Aliases


            type Animal = {
            name: string
            }

            type Bear = Animal & { 
            honey: boolean 
            }

            const bear = getBear();
            bear.name;
            bear.honey;
                
       

### different :

 interface:

            interface Window {
            title: string
            }

            interface Window {
            ts: TypeScriptAPI
            }

   type:
   
                type Window = {
                title: string
                }

                type Window = {
                ts: TypeScriptAPI
                }

                // Error: Duplicate identifier 'Window'.

        
	

### different another example :

type 

    type x = {
     a: string ;
     b: string ;
     
     }
     
     type y = x & {
      c : string ;
      d : string ;
      
      }
      
 interfacce 
 
    interface x {
    
        a : string ;
	b : string ;
	}
	

	
     interface y extends x {
      c : string ;
      d : string ;
      }
   
    

 
### 7th example : generic Type 


            function greet<Str extends string>(s: Str) {
            console.log("Hello, " + s);
            }
            
            greet("world")



### 8 th example : Array 


            const num : number [ ] = [1,2,3,4]
            const strings :string [ ] = [ " hello " , "world" ]

            const objects : object [ ] = [ { key: 'value' } ]
