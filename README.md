                                                                           DAY -5
                                                           
                                                             USING ANONYMOUS AND IIFE FUNCTIONS|
                                                            


A. PRINT ODD NUMBERS IN AN ARRAY.


CODE:  USING IIFE(Immediately Invoked Function Expression)


     (function display(numbers=[])
         {
                     let s1=""
                     for(var i in numbers)           
                         {
                                    if(numbers[i]%2!=0)    // Logic to identify ODD numbers in an Araay
                                      {
                                                  s1=s1+" "+numbers[i]
                                       }
      
                          }
                 console.log(`odd numbers are :${s1}`)  //Printing ODD numbers

          })([2,3,4,5,6,7,8,9])

 OUTPUT:
 ...................
     odd numbers are : 3 5 7 9


CODE:   USING ANONYMOUS FUNCTION
....................................
let display= function (numbers=[])
         {
                     let s1=""
                     for(var i in numbers)           
                         {
                                    if(numbers[i]%2!=0)    
                                      {
                                                  s1=s1+" "+numbers[i]
                                       }
      
                          }
                 console.log(`odd numbers are :${s1}`)  

          }

    display([2,3,4,5,6,7,8,9])

   OUTPUT:
..............................
    odd numbers are : 3 5 7 9
.......................................................



 CODE:   USING ANANYMOUS FUNCTION


 let titlecaps= function (values=[])
        { 
               let s3=[]
              for(var index in values)
                  {
                       let s1=values[index].split("")
                        let s2=""                                                                                                                                                           
             
                      for(var i=1;i<s1.length;i++)      
                          {
                                 s2=s2+s1[i]                    
                          } 

                     s3=s3+s1[0].toUpperCase()+s2+" "  +a v a
                                                                                                                                                                                                                          

                  }
              console.log("Strings with Titlecaps: ",s3)
       }

    titlecaps(["Abdul","Hadhi","full","stack","developer"])


   OUTPUT:
..........................
     Strings with Titlecaps:  Abdul Hadhi full stack developer


 ...........................................................................

( function titlecaps (values=[])
     { 
            let s3=[]
           for(var index in values)
               {
                  let s1=values[index].split("")   
                     let s2=""                                                                                                                                                           
          
                   for (var i=1;i<s1.length;i++)      
                       {
                              s2=s2+s1[i]                      
                       } 

                   s3=s3+s1[0].toUpperCase()+s2+" "  
                                                                                                                                                                                                                           
                }
       console.log("Strings with Titlecaps: ",s3)

    }(["Abdul","Hadhi","full","stack","developer"])   

   OUTPUT:
........................
    Strings with Titlecaps:  Abdul Hadhi full stack developer



C.SUM OF ALL NUMBERS IN AN ARRAY
...................

    CODE: USING  ANONYMOUS  FUNCTION
     -------

           let sum=function(numbers=[])   
                {
    
                           for(var number of numbers) 
                                {
                                            sum=sum+number  
                                 }

                            return sum                         
                  }
            console.log(`sum of all elements in an array : ${sum([20,30,40,50,60,70,80])}`)  //Calling Anonymous function
    

     OUTPUT:
     ............................

         sum of all elements in an array : 350


 CODE:  USING IIFE FUNCTION
 

  (function sum(numbers=[])    
     {
                 let sum=0                                

                for(var number of numbers) 
                     {
                                 sum=sum+number 
                 
                 console.log(`sum of all elements in an array : ${sum}`)                     
       
     }([20,30,40,50,60,70,80]))  


     OUTPUT:
      ----------

         sum of all elements in an array : 350
...................................................
 
 D.RETURN ALL PRIME NUMBERS IN AN ARRAY
 .......................................
 
  CODE :  USING ANONYMOUS FUNCTION
   -------

          let prime=function (numbers=[])        
                {
                         let count
                         let s1=""
                         for( var i=0;i<numbers .length; i++ )    
                              {
                                      count=0
                                      for(var j=1;j<=numbers[i];j++)  
                                          {
                                                  if(numbers[i]%j==0)    
                                                  
                                                  whether  2 divisible by 1,2( J -- up to numbers[0])
                                                      {  
                                                                  count=count+1   
                
                                                       }
                                              }

                                      if(count==2)            
                                        {                            
                                                s1=s1+" " +numbers[i]
                                        }
      
                                }

                          return s1                     
                   }

             console.log(`Prime Numbers in given array are: ${prime([2,3,4,5,6,7,8,9,10,11])}`)


     OUTPUT:
      ----------
 
           Prime Numbers in given array are:  2   3   5   7   11


CODE: USING IIFE FUNCTION
----------------------------------------------

 (function prime(numbers=[])       
                {
                         let count
                         let s1=""
                         for( var i=0;i<numbers .length; i++ )     
                              {
                                      count=0
                                      for(var j=1;j<=numbers[i];j++)  
                                          {
                                                  if(numbers[i]%j==0)     
                                                                                        
                                                      {  
                                                                  count=count+1   
                
                                                       }
                                              }

                                      if(count==2)            
                                        {                          
                                                s1=s1+" " +numbers[i]
                                        }
      
                                }

                          
                          console.log(`Prime Numbers in given array are: ${s1}`) 
                                                             
  
                   }([2,3,4,5,6,7,8,9,10,11]))

     OUTPUT:
      ----------
 
           Prime Numbers in given array are:  2   3   5   7   11

...............................................

  E. RETURN ALL PALINDROMES IN AN ARRAY
  -----------------------------------------------------------

  CODE:  USING IMMEDIATELY INVOKED FUNCTION EXPRESSION  ( IIFE )
   -------
   
     (function palindrome (values=[])
       {
                 let s3=[]
                 for(var index in values)
                     {
                               let s1=values[index].split("")  .
                               let s2=values[index].split("")
                                  let n1=s1.length
                                  let n2=s2.length           .

                                 let count=0                                      
                                 for(var i=0; i<n1&&n2>=0; i++,n2--)  
                                     {
                                          if(s1[i]==s2[n2-1])           
                                             { 
                                                     count=count+1     
                                              }
                                      }

                            if(count==n1)                       
                              {
                                      s3=s3+s1.join("")+" "  
  
                        }

              console.log(`palindromes in given array are :`)
              console.log(`[ ${s3} ]`)

                                              
            })(["Abdul","Hadhi","refer","abdul","dominar","random","level","civic"]) 

  

CODE:  USING ANONYMOUS FUNCTION
...........................................

 let palindrome =function (values=[])
       {
                 let s3=[]
                 for(var index in values)
                     {
                               let s1=values[index].split("")  
                               let s2=values[index].split("")
                                  let n1=s1.length
                                  let n2=s2.length           

                                 let count=0    
                                 for(var i=0; i<n1&&n2>=0; i++,n2--)
                                     {
                                          if(s1[i]==s2[n2-1])          
                                             { 
                                                     count=count+1     
                                              }
                                      }

                            if(count==n1)                         
                              {
                                      s3=s3+s1.join("")+" " 
                                }
  
                        }

              console.log(`palindromes in given array are :`)
              console.log(`[ ${s3} ]`)

                                            
            }
            
            palindrome  (["Abdul","Hadhi","refer","Abdul","dominar","random","level","civic"])

.............................................................................................
F.  RETURN THE MEDIAN OF TWO SORTED ARRAYS OF SAME SIZE
 ------------------------------------------------------------------------------------------------

CODE :USING ANONYMOUS FUNCTION
---------

 let median= function (array1,array2)
     {
           
           array1=[...array1,...array2]         
           console.log(`Unsorted array after merging two arrays :${array1}`)
           let temp
            
         /*  array1=array1.sort((a,b)=>a-b)   
           console.log(array1)  */

              for(var i=0;i<array1.length;i++)  
                  {
                           for(var j=i;j<array1.length;j++)
                                {
                                           if(array1[i]>array1[j+1])   
                                              {
                                                   temp=array1[i]              
                                                   array1[i]=array1[j+1]    
                                                   array1[j+1]=temp       

                                              }                                    /
                                }
                    }
            console.log(`sorted array is: ${array1}`)
         
              let n=array1.length                                      
              let median                                                 
              if(n%2==0)                            
                {
                     let x=n/2                         
        median=(array1[x-1]+array1[x])/2   
                 }

              else if(n%2!=0)     
                {
                     let x=Math.round(n/2) 
                    median=array1[x-1]      
                 }

            return median               
   
    }
 
     console.log(`Median of two sorted arrays of same size is: ${median([1,3,5,7,9],[2,4,6,8,10])}`)

    OUTPUT:
    -------------

                  Unsorted array after merging two arrays :1,3,5,7,9,2,4,6,8,10

                 sorted array is: 1,2,3,4,5,6,7,8,9,10

                 Median of two sorted arrays of same size is: 5.5


CODE:USING IMMEDIATELY INVOKED FUNCTION EXPRESSION(IIFE)
.............................................................................
 ( function median(array1,array2)
     {
           
           array1=[...array1,...array2]
           console.log(`Unsorted array after merging two arrays :${array1}`)
           let temp
            
          /* array1=array1.sort((a,b)=>a-b)
           console.log(array1)*/
         
           for(var i=0;i<array1.length;i++)
               {
                       for(var j=i;j<array1.length;j++)
                           {
                                  if(array1[i]>array1[j+1])
                                    {
                                        temp=array1[i]
                                        array1[i]=array1[j+1]
                                        array1[j+1]=temp

                                    }
                           }
            }
         console.log(`sorted array is: ${array1}`)
        let n=array1.length
        let median
        if(n%2==0)
         {
           let x=n/2  
           median=(array1[x-1]+array1[x])/2
         }

         else if(n%2!=0)
         {
           let x=Math.round(n/2)
           median=array1[x-1]
         }

         console.log(`Median of two sorted arrays of same size is: ${median}`)

        }([1,3,5,7,9],[2,4,6,8,10]))

 OUTPUT:
 

                  Unsorted array after merging two arrays :1,3,5,7,9,2,4,6,8,10

                 sorted array is: 1,2,3,4,5,6,7,8,9,10

                 Median of two sorted arrays of same size is: 5.5


G..REMOVE DUPLICATES FROM AN ARRAY 

 
  CODE:USING ANONYMOUS FUNCTION
   --------

    let duplicates=function (values=[])
        {

               for(var i=0;i<values.length;i++)   
                   {
                            for(var j=i+1;j<values.length;j++)
                                {
                                       if(values[i]==values[j])      
                                                 {
                                                          values.splice(j,1)   
                                                  }
                                 }
                    }
         return values

      }
   console.log("Unique values in array are:")
   console.log(duplicates([1,2,1,3,4,5,4,3,5,6]))
     
      OUTPUT:
      
               Unique values in array are:
  
                      [1, 2, 3, 4, 5, 6]


CODE:USING IMMEDIATELY INVOKED FUNCTION EXPRESSION
 
  (function duplicates (values=[])
        {

               for(var i=0;i<values.length;i++)   
                   {
                            for(var j=i+1;j<values.length;j++)
                                {
                                       if(values[i]==values[j])       
                                                 {
                                                          values.splice(j,1)   
                                                          }
                                 }
                    }
         
      console.log(`Unique values in array are: ${values}`)

      }([1,2,1,3,4,5,4,3,5,6]))

     
      OUTPUT:
       -----------
               Unique values in array are:
  
                      [1, 2, 3, 4, 5, 6] 


      
  H. ROTATE ELEMENTS IN AN ARRAY BY K TIMES


 CODE:USING ANONYMOUS FUNCTION
  --------

     let rotate=function (elements,k)                   
                                     {
                                              for(var i=0;i<k;i++)      
                                                   {
                                                              leftrotate(elements)  
                                                              }

                                         function leftrotate(elements)           
                                                      {
                                                             var temp=elements[0]   
              
                                                            for(var i=0;i<elements.length-1;i++) 
                                                                {

                                                                     elements[i]=elements[i+1]       
                 
                                                                 }
                                                            elements[elements.length-1]=temp   AY

                                                        }
    
                                        return elements
                              }

     console.log(`Left rotating elemnts :${rotate([3,4,5,6,7],2)}`)

   OUTPUT:


    Left rotating elemnts :5,6,7,3,4


  CODE:USING IIFE FUNCTION


                            (function rotate (elements,k)                 
                                     {
                                              for(var i=0;i<k;i++)          
                                                   {
                                                              leftrotate(elements)  
                                                    }

                                         function leftrotate(elements)           
                                                      {
                                                             var temp=elements[0]    
              
                                                            for(var i=0;i<elements.length-1;i++) 
                                                                {

                                                                     elements[i]=elements[i+1]     
                 
                                                                 }
                                                            elements[elements.length-1]=temp    

                                                        }
    
                                        
                                        console.log(`Left rotating elemnts :${elements}`)

                              }([3,4,5,6,7],2))


     OUTPUT:
   ---------------

    Left rotating elemnts :5,6,7,3,4
         
                                                                     USING ARROW FUNCTION  
 .................................................................................................................................................                                                                    
                                                               
a. Print odd numbers in an array


 CODE:            ARROW FUNCTION    '  => '
  -------  

 let display=  (numbers=[])=>
     {
                     let s1=""
                     for(var i in numbers)           
                         {
                                    if(numbers[i]%2!=0)    
                                      {
                                                  s1=s1+" "+numbers[i]
                                       }
      
                          }
                 console.log(`odd numbers are :${s1}`)  

      }

display([2,3,4,5,6,7,8,9])


OUTPUT:
------------

odd numbers are : 3 5 7 9


b.Convert all the strings to title caps in a string array


CODE:

let titlecaps= (values =[])=>
        { 
               let s3=[]
              for(var index in values)
                  {
                       let s1=values[index].split("")
                        let s2=""                                                                                                                                                           
             
                      for(var i=1;i<s1.length;i++)      
                          {
                                 s2=s2+s1[i]                     
                          } 

                     s3=s3+s1[0].toUpperCase()+s2+" "                                                         
                  }
              console.log("Strings with Titlecaps: ",s3)
       }

    titlecaps(["java","javascript","ecmascript","nodejs","react"])

 OUTPUT:
 ------------

Strings with Titlecaps:  Java  Javascript   Ecmascript   Nodejs   React


 C.Sum of all numbers in an array
-----------------------------------------

CODE:
---------

 let sum=(numbers=[])  =>  //ARROW function
     {
                 let sum=0                                

                for(var number of numbers) 
                     {
                                 sum=sum+number   
                      }

                 return sum                          
       }
 console.log(`sum of all elements in an array : ${sum([20,30,40,50,60,70,80])}`)  

  OUTPUT:
..................
sum of all elements in an array : 350



d.Return all the prime numbers in an array


CODE:


 let prime=  (numbers=[]) =>     
                {
                         let count
                         let s1=""
                         for( var i=0;i<numbers .length; i++ )     
                              {
                                      count=0
                                      for(var j=1;j<=numbers[i];j++)  
                                          {
                                                  if(numbers[i]%j==0)     
                                                                                         
                                                      {  
                                                                  count=count+1    
                
                                                       }
                                              }

                                      if(count==2)           
                                      {
                                                s1=s1+" " +numbers[i]
                                        }
      
                                }

                          return s1                     
                   }

             console.log(`Prime Numbers in given array are: ${prime([2,3,4,5,6,7,8,9,10,11])}`)

  OUTPUT:

   Prime Numbers in given array are:  2 3 5 7 11


e. Return all the palindromes in an array
 

CODE:


 let palindrome = (values=[])   =>
       {
                 let s3=[]
                 for(var index in values)
                     {
                               let s1=values[index].split("")  
                               let s2=values[index].split("")
                                  let n1=s1.length
                                  let n2=s2.length            

                                 let count=0    
                                 for(var i=0; i<n1&&n2>=0; i++,n2--)
                                     {
                                          if(s1[i]==s2[n2-1])          
                                             { 
                                                     count=count+1      
                                              }
                                      }

                            if(count==n1)                       
                            {
                                      s3=s3+s1.join("")+" "  
                                }
  
                        }

              console.log(`palindromes in given array are :`)
              console.log(`[ ${s3} ]`)

            }
            palindrome  (["Abdul","Hadhi","refer","Abdul","dominar","random","level","civic"])


