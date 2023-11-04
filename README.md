# String_Manipulate
#### Reverse string
```
function reverseString(str){
  return str.split("").reverse().join("")
}
console.log(reverseString("tech"))
```
---
```
function reverseStringUsingLoop(str){
  let reverse = ''
  for(let char of str){
    reverse = char + reverse
  }
  return reverse
}
console.log(reverseStringUsingLoop("world"))
```
---
####  Check if a string is a palindrome.
```
function palindrome(str) {
  const rev = str.split("").reverse().join("");
  return rev === str;
}

console.log(palindrome("nayan"));
```
---`
####  Count the number of vowels in a string.
```
function countVowels(str){
  let vowel = ['a','e','i','o','u'];
  let count = 0
  for(let vo of str.toLowerCase()){
     if(vowel.includes(vo)){
       count++
     }
  }
  return count
}
console.log(countVowels('dhanaraj'))
```
---
####  Count the number of words in a sentence.
```
function countWords(str){
  let splitArr = str.split(" ")
  return splitArr.length
}
console.log(countWords("i am Dhanaraj"))
```
---
####  Capitalize the first letter of each word in a sentence.
```
function capitalizeFirstLetter(str) {
  let splitArr = str.split(" ");
  for (let i = 0; i < splitArr.length; i++) {
    splitArr[i] = splitArr[i].charAt(0).toUpperCase() + splitArr[i].slice(1);
  }
  return splitArr.join(" "); 
}

console.log(capitalizeFirstLetter("dhanu ddnjnj dnjnjd"));
```
---
####  Remove all whitespace from a string.
```
function removeWhiteSpace(str){
  let remove = str.trim()
  return remove
}
console.log(removeWhiteSpace("   dhanu   "))
```
---
####  Replace all occurrences of a substring in a string.
```
function replaceAllOccurrences(inputString, search, replacement) {
  ####  Use a regular expression with the 'g' flag to replace all occurrences
  const regex = new RegExp(search, 'g');
  const result = inputString.replace(regex, replacement);
  return result;
}

const originalString = "This is an example, and this example is just an example.";
const searchString = "example";
const replacementString = "sample";

const modifiedString = replaceAllOccurrences(originalString, searchString, replacementString);

console.log(modifiedString);
```
---

####  Find the longest word in a sentence.
```
function longestString(str){
  let longest = ''
  let words = str.split(' ')
  for(let word of words){
    if(word.length  >  longest.length){
      longest = word
    }
  }
  return longest
}
console.log(longestString("i am dhanu"))
```
---

####  Check if a string contains only digits.
```
function checkIfNum(str){
  for(let i=0;i<str.length;i++){
    if(isNaN(str[i])){
      return false
    }
  }
  return true
}
console.log(checkIfNum("1234sss"))
```
---

####  Check if a string contains only alphabetic characters.

---

####  Check if two strings are anagrams of each other.
---

####  Count the occurrences of a specific character in a string.
---

####  Find the first non-repeated character in a string.
---

####  Remove duplicates from a string.
---

####  Reverse the words in a sentence.
---

####  Convert a sentence to title case.
---

####  Check if a string is a valid email address.
---

####  Check if a string is a valid URL.
---

####  Find the common characters between two strings.
---

####  Check if a string is a valid IPv4 address.
---


