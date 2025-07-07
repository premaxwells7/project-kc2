FIRST
function factorial(num) {
  let result = 1;
  for (let i = 1; i <= num; i++) {
    result *= i;
  }
  return result;
}

// Example:
console.log(factorial(6)); // Output: 720

SECOND
function findLargestNumber(arr) {
  let largest = arr[0];
  for (let i = 1; i < arr.length; i++) {
    if (arr[i] > largest) {
      largest = arr[i];
    }
  }
  return largest;
}

// Example with random numbers:
let randomNumbers = [14, 33, 100, 29, 88, 65];
console.log("Array:", randomNumbers);
console.log("Largest:", findLargestNumber(randomNumbers)); // Output: 100

THIRD
function countConsonants(str) {
  const vowels = ['a', 'e', 'i', 'o', 'u'];
  let count = 0;

  str = str.toLowerCase();

  for (let i = 0; i < str.length; i++) {
    const char = str[i];
    if (/[a-z]/.test(char) && !vowels.includes(char)) {
      count++;
    }
  }

  return count;
}

// Example:
console.log(countConsonants("Prex Maxwell")); // Output: 7

FOURTH
function multiplicationTable(num) {
  for (let i = 1; i <= 12; i++) {
    console.log(${num} X ${i} = ${num * i});
  }
}

// Example:
multiplicationTable(7);

// Output:
// 7 X 1 = 7
// 7 X 2 = 14
// ...
// 7 X 12 = 84

FIFTH
function reverseWithCallback(str, callback) {
  const reversed = str.split('').reverse().join('');
  callback(reversed);
}

// Example:
reverseWithCallback("prex", function(result) {
  console.log("Reversed string:", result);
});

// Output:
// Reversed string: xerp
