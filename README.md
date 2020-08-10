
## convert minutes to seconds function
 Create a function using built-in math object Math.floor,to convert minutes to seconds in javascript. 
In this function, which  will pass minutes and it returns the value in seconds. 

  ## Syntax

> convertMinutestoSeconds(minutes)
### Parameters

   **number** : `minutes`

 The function accepts an integer numbers.

### Return Value: `Number`

  returns an integer
 
## Examples

```js
convert(5) ➞ 300

convert(4) ➞ 240
```
**The function is below:**
```js
     function convertMinutestoSeconds(minutes) {
          
          // use built-in object math.floor
         
          return Math.floor(minutes * 60);
          
          };
```
Test.assertEquals(convert(5), 300)
Test.assertEquals(convert(4), 240)
Test.assertEquals(convert(7), 420)
_____
## Farm problem
Create a function to count total of animals legs inside object array which have keys and its value,in this function, will pass animals and its return the total sum of each key value * the number of legs for each type of animals inside the object array. 


 ## Syntax

> function count_leg(animals)
### Parameters

   **number** : `animals`

 The function accepts an integer numbers.

### Return Value: `Number`

  returns an integer
 
## Examples

```js
{'ducks': 1, 'sheeps' : 1, 'pigs' : 1}
Should return: 10 

{'ducks': 24, 'sheeps' : 12, 'pigs' : 13}
Should return: 148
```
**The function is below:**
```js
    function count_leg(animals){

      // get key value of the object array 

    return animals.ducks*2 + animals.sheeps*4  + animals.pigs*4;
        };
```
___
# get odd occurrence
     create a function that takes a sequence of numbers and finds the integer which appears an odd number of times. in this function, using for loop to pass all items inside the array if repeated odd number then return odd number. 


  ## Syntax

> getOddOccurrence = (arr) =>
### Parameters

   **number** : `arr`

 The function accepts an integer numbers.

### Return Value: `Number`

  returns an integer
 
## Examples

```js
[2, 3, 5, 4, 5, 2, 4, 3, 5, 2, 4, 4, 2 ]
Should return: 5 (the only odd number)

[2, 5, 5, 4, 5, 2, 4, 3, 5, 2, 4, 4, 2 ]
Should return: 3 (the only even number)
```
 **The function is below:**   
 ```js
     let getOddOccurrence = (arr) => {
    var count = 0;  // we have count already declared and assigned
    

    for(var i = 0; i<arr.length; i++){  // check existing variable for each i in array length 
       
      for(var j = 0; j <arr.length; j++){
        if(arr[i] == arr[j]){
          count++;
        }
      }
       
      if(count % 2 != 0 ){  // check odd items in array
        
        return arr[i]; // return odd element 
      }
    }
  };
```
  _____
# count progress days
   Create a function that takes in a list of miles run every Monday and returns John' total number of progress days. in this function, we pass all days in for looping to check all items in array if they pass the test  return count of total days.

## Syntax

> function count_proregss(times)
### Parameters

   **number** : `times`

 The function accepts an integer numbers.

### Return Value: `Number`

  returns an integer
 
## Examples

```js
[3,4,3,6,3,4]
Should return: 3 (total progress days)

[8,10,11,8,7,9,9,10]
Should return: 4 (total progress days)
```
**The function is below:**
```js
    function count_proregss(times){
     
       let days=0; // set the days that will be the output

	   for(i =1; i<times.length; i++){ // check for each item i in the times
        
		if(times[i]>times[i-1]){ // check if new i bigger than last i item in array
			days++;  //  increments the counter
		} 
	}
	return days; 
     };
```
```js
const chai = require("chai");
const assert = chai.assert;
chai.config.truncateThreshold = 0;

describe("upArray()", () => {
  it("should handle basic tests", () => {
    assert.deepEqual(count_proregss([4,4,6,5,3]), 1);
    assert.deepEqual(count_proregss([8,10,11,8,7,9,9,10]), 4);
    assert.deepEqual(count_proregss([5,5,5]), 0);
    assert.deepEqual(count_proregss([13,15,16,16,14,12,15,17,13]), 4);
    
  });
});
```
_____
# find distinct number

 > create a function which find  distinct numbers inside array and return these two numbers. in this function,Take the check at the end of the inner loop and check the index j with the length of the array l, and if equal push the value to unique array.

 ## Syntax

> find_distinct_element(arr)
### Parameters

   **number** : `arr`

 The function accepts an integer numbers.

### Return Value: `Number`

  returns an integer
 
## Examples

```js
[24,7,5,88,96,88,5,7,24,21]
Should return: [96,21] (new array)

[24,5,88,96,96,88,5,7,21,21]
Should return: [24,7] (new array)
```
**The function is below:**
```js

function find_distinct_element(arr) {
   
    
    let l = arr.length, i, j,  // Set the variables.


           let unique = []; // set new array.
        
         
        for (i = 0; i < l; i++) {   // Start looking the array for distinct items.

            for (j = 0; j < l; j++) {

                if (i === j) { // Check i and j and if equal continue the (inner) loop.
                    continue;
                }

                if (arr[i] === arr[j]) { // Check the value at i and j in the (inner) loop, because a duplicate is found.

                    break; // if there is not duplicated stop looping.
                }
            }
            if (j === l) {  // Check j and l and if equal.

                unique.push(arr[i]); // push odd  value in unique array.
            }
        }
        return unique;
    };

```

I'd like to expand my knowledge,skills and learning as much as I can, as quickly as I can, by end AI Bootcamp. From there, I'd seek out opportunities  to expand my knowledge through training and educational opportunities to support my career opportunities. I'd love to participate in at least one project related for big data to shape my skills in field of AI & machine learning, prepared me well for labor market to land a good job.  
___
First I would like to express my appreciation for this opportunity to apply for AI Bootcamp, In fact, as I have read about this program, I found it very interesting and
very promising to increase my vision and skills in big data field.
Currentlly, I doing 7 months intensive program in software development at HackYourFuture
coding school in Brussel,provided me with a strong footing in the theoretical concept of Computer Science and Software Engineering. from there, i figure out the value of big data sector to solve any problem now days.
While AI Bootcamp offering both depth and extensiveness across this field, these courses put into perspective
the relevance of big data and the application of its fundamentals to the problems
faced by the real world.
Therefore, I can acknowledge that further development of my knowledge base of big data is essential for my career path towards become Data Engineer
I would offer my leadership skills, a strong educational background and desire to go one-step
further than the others would.
I have the right academic record, the right skills and attitude to succeed and I am convinced
that this program is the right stepping-stone for my professional ambitions.
Once again I am grateful for considering my application and I look forward to a favourable
reply.
