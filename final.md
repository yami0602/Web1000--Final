# Final exam

## Instructions

Create a github repository called web1000-final. **If you do not name your repository correctly and don't submit it to canvas you will receive a zero. Looking at you, Arnaldo.**

In your repository, create a file called testAnswers.txt and **copy and paste all the questions in there.**

Answer each question right below the question text.

## Questions

1. What are the four steps of mergesort?

The four steps of the mergesort: 
 
Divide 
Sort 
Combine 
Return 

2. Using JavaScript, generate a random number between 50 and 100.

Answer: Math.floor(Math.random() * 50 + 50;)

3. Using Javascript, generate a random number between -100 and 100.

Answer: Math.floor(Math.random() * -200 + 100)

4. Write a coin flip function. It should return the string "heads" half the time and the string "tails" the other half
```javascript


  function coinFlip(){

	    return (Math.floor(Math.random() * 5) == 0) ? 'heads' : 'tails';

	}

	coinFlip();
  
```


5. Re-state the following expression without using negation:
  !(10 > x)

  (10 <= x)

6. Re-state the following expression without using negation:
  !(a > 10 && b <= 5)

  (a <= 10 || b > 5)

7. Re-state the following expression without repeating variable a:
  (a && x <= 10) || (a && y < 0)

  !(a || x > 10) && !(a || y >= 0)

8. Re-state the following expression without negations:
  !( (a > 10) || (b > 10) || (c > 10) || (isAdmin) )

  ((a <= 10) && !(b <= 10) && !(c <= 10) && !(isAdim))

9. Write a function which, given a 2-d array of strings, returns the concatenation of all the strings.
```javascript
 
 var ret = [[['Basketball'],['Softball']],[[" all day"], ['every day']]];  

    function twoConcat(arr) {
      var ret = [];
       
        for(var i = 0; i < arr.length; i++) {
            if(Array.isArray(arr[i])) {
                ret = ret.concat(twoConcat(arr[i]));
            } else {
                ret.push(arr[i]);
            }
        }
        return ret;
    }


10. Write a function which, given a 2-d array and another value x, returns true if x is present in the 2-d array, and false otherwise.
``

function containsElement(arr, x) {
    for (var r = 0; r < arr.length; r++) {
        for (var c = 0; c < arr[r].length; c++) {
            if (arr[r].indexOf(x) > -1) {
                return true;
            }
        }
    }
    return false;
};

containsElement([
    ["Soccer", "Tennis"],
    ["Football", "Softball"]
], "Basketball");
```



11. Write a function which, given an two sorted arrays of sizes m and n, returns a larger sorted array of size m+n. This function must work in O(m+n) time.

12. Given the following edge list, draw the graph. Use MS Paint and include the file in your repo.

```javascript
E = [[1,2], [2,3], [4,5], [2,4], [1,5]  ]
```
            Answer: powerpoint(slide 8)
```

13. Given the following adjacency Matrix, determine whether the graph is directed or undirected and draw it.

Answer; PowerPoint slide 7

```javascript
M = [
  [0,0,1,0,1],
  [0,0,0,0,1],
  [0,1,0,0,0],
  [0,1,0,0,0],
  [0,0,0,0,1],
]
```

14. For exercises 9 and 10, if you assume that n is the size of one side of the matrix, what is the time complexity (Big Oh) of the algorithms you wrote?

Answer: The time complexity of the algorithms i wrote is o(n^2)

15. What is the time complexity of the following function?

Answer: O(n^2)

```javascript
  function thugPop(arr){
    var ret = [];
    for (var i === 0; i < arr.length; i++){
      if (arr[i] % 15 == 0) ret.push('thugPop');
      else if (arr[i] % 5 == 0) ret.push('thug');
      else if (arr[i] %3 == 0 ) ret.push('pop');
      else ret.push(arr[i]);
    }
    return ret;
  }
```

16. What is the time complexity of the following function?

Answer: O(n)

```javascript
  function thugify(schoolList){
    return schoolList.map(function(schoolObj){
      var school = Object.assign({}, schoolObj);
      school.students.forEach(function(student){
        if (Math.random() > 0.5){
          student.lastName += 'dogg';
        }
        else {
          student.firstName = "lil' "+ student.firstName;
        }
      });
    });
  }
```

17. What is the time complexity of the following function?
Answer: O(n)

```javascript
  function countRepeats(strArr){
    var repeats = 0;
    strArr.forEach(function(str, index){
      var currentRepeats = strArr.filter(function(innerStr, idx){
        return (innerStr === str && index != idx)
      });
      if (currentRepeats.length > 0){
        repeats++;
      }
    });
    return repeats;
  }
```

18. What are the main operations of a stack?

Answer:  (to add data) .push() Method adds elements to the end of the array and then          returns the new length of the array

          (to remove data) .pop() Method removes the last element from the array, then returns the lenght of the new array.


19. What are the main operations of a queue?

Answer: (to add data) .enqueue() Method adss a node to the back of the queue.
                      .dequeue(). Methods removes a node from the front of the queue.




20. What is the runtime of bubblesort? How does it work?

The run timr for bubbblesort is o(n^2) - linear


21. Create a personal website and upload it so that it is accessible at yourdomain.fvi-grad.com.  
    1. The website must have your name, contact information, skills, and at least two links to portfolio items you are hosting on fvi-grad.
    2. The website must not be in a subdirectory of the document root. ie. It needs to be accessible by going to yourusername.fvi-grad.com/ without anything after the slash.
    3. You can and should use a template
    4. Include the link to your website in your answers document
