# Mystery Function

What does the `mystery()` function in the following piece of code do? Add your
answer to this markdown file.

```javascript
function mystery(a) {
    if(a.length == 1) return a[0];
    var foo = mystery(a.slice(1, a.length))
    if(foo > a[0]) return foo;
    else return a[0];
}
```

This mystery function compares every element of the array and gives the largest one by recusively reducing the array and comparing values
if(a.length == 1) return a[0] is the base case where if there is only one element, it is by default the largest element
var foo = mysetry(a.slice(1, a.length)) is where the array is recursively reduced by removing the first element 
if (foo > a[0]) return foo; compares the first element with the result of the recursive call so if foo is larger than a[0] the function returns foo otherwise it returns a[0]

Sources:
I looked at https://www.javatpoint.com/array-slicing-in-java as a reminder for what slicing does

Plagarism statement:
"I certify that I have listed all sources used to complete this exercise, including the use of any Large Language Models. All of the work is my own, except where stated otherwise. I am aware that plagiarism carries severe penalties and that if plagiarism is suspected, charges may be filed against me without prior notice."
This was my submission from last semester
