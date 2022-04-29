Method 1  😐️
--------------------------  Complexity(  O(1)  )

var leftRotate = (arr, n, d) => {
 var temp = arr.slice(0, d);
 var newArr = arr.slice(d);
 return newArr.concat(temp);
}

Method 2 😐️
----------------------------

var arrayRotate = (arr, n, d) => {
for(let i=0; i<d; i++) {             // O(n)
  leftRotate(arr, n);
 }
 return arr;
}

var leftRotate = (arr, n) => {
 var temp = arr[0];
 for(let i=0; i<n-1; i++) {        //O(n)
  arr[i] = arr[i+1];
 }
 arr[n-1] = temp;
}


Method 3  😐️ Pending
----------------------------
