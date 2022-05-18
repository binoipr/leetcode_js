
----character count using forEach-----

function charCount(str) {
let res = {};
  str.split("").forEach((s)=> {
  return res[s] ? res[s]++ : res[s] = 1;
  })
 return res;
}

-timeComplexity = O(n); 
-spaceComplexity = O(n); // not sure


-----using Array.from().reduce -----

function charCount(str) {
var count = Array.from(str).reduce((accumulator, ch)=> {
 if(ch in accumulator) {
  accumulator[ch]++;
 } else {
  accumulator[ch] = 1;
 }
 return accumulator;
}, {})
return count;
}

console.log(charCount("abcsddesaacvfswsx"))




