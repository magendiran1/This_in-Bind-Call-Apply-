# This_How its working in=>-Bind-Call-Apply-


# Bind

          ** we are going to see Example **
 
----------------------------------------------------------------------------------------------------------------------------

// we are going to see [Bind] how its working and what is purpose


**var person ={
    firstName:"magendiran",
    lastName:"R",
    gender :"Male"
    }
    
**function getFullName(){ 
      return   "Hello " +this.firstName +" "+ this.lastName+"Welcome"
     }
    
  # console.log(getFullName.bind(person)())
  
    //why i have keep the [function call]=() because bind will execute immediately. 
    //it will create new function then we have call when its required.

*       Like this we have use if we are not user ()
   # let mybind =getFullName.bind(person)
   # console.log(mybind())
    
----------------------------------------------------------------------------------------------------------
# Call


#   syntax for Call 

function.call(this,argu1,argu2,argu3)

**let person2 ={
    firstName:"Thalapathi",
    lastName:"Vijay",
    gender :"Male"
    }



**function totalHitFlopMovies(a,b,c,d) {
return "Hi everyone" +this.firstName +this.lastName+"Total Hit Mobvies="+ (a+b) +" Flop movies is "+(c+d)
}

console.log(totalHitFlopMovies.call(person2,25,40))--->person2 is this, here i have gave only two argument so in the function its consider only a,b

console.log(totalHitFlopMovies.call(person2,25,40,0,0))


---------------------------------------------------------------------------------------

# Apply 


#   syntax for Call 

function.call(this,[argu1,argu2,argu3])


**let person3 ={
    firstName:"Thalapathi",
    lastName:"Vijay",
    gender :"Male"
    }


**function totalHitFlopMovies(a,b,c,d) {
return "Hi everyone" +this.firstName +this.lastName+"Total Hit Mobvies="+ (a+b) +" Flop movies is "+(c+d)
}



console.log(totalHitFlopMovies.apply(person3,[25,40]))

console.log(totalHitFlopMovies.apply(person3,[25,40,0,0]))

--------------------------------------------------------------

# Differene b/w Call vs Apply 

** In the call argument will pass in seperate like 2,3,4 but in Apply the argument will pass as an ARRAY [2,3,4,5]










