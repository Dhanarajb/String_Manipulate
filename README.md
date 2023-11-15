# String_Manipulate
#### Reverse string
```
function reverseString(str){
  return str.split("").reverse().join("")
}
console.log(reverseString("tech"))
```
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
---
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
```
 function checkAlp(str){
   for(let item of str){
     if(!isNaN(item)){
       return false
     }
   }
   return true
 }
 console.log(checkAlp("snsn"))
```
---

####  Check if two strings are anagrams of each other.
```
function angramString(str1,str2){
     let strMatch1 = str1.split("").sort().join("")
     let strMatch2 = str2.split("").sort().join("")
     return strMatch1 === strMatch2
   }
   console.log(angramString("silent", "listen"))
```
---

####  Count the occurrences of a specific character in a string.
```
 function countOcc(str){
     let obj={}
     for(let char of str){
       !obj[char]? (obj[char]=1):obj[char]++
     }
     return obj
   }
   console.log(countOcc("njdjnjndjn"))
```
---

####  Find the first non-repeated character in a string.
```
function nonRepeat(str){
     let obj = {}
     for(let char of str){
       !obj[char] ? (obj[char]=1) : obj[char]++
     }
     console.log(obj)

     for(let char of str){
       if(obj[char]===1){
         return char
       }
     }
     return null
   }
   console.log(nonRepeat("dnknkknf"))
```
---

####  Remove duplicates from a string.
```
let dup = ""
     for(let char of str){
       if(dup.includes(char)==false){
         dup += char
       }
     }
     return dup
   }
   console.log(duplicateString("dhanaasjs"))
```
```
function removeDuplicates(inputString) {
    let uniqueCharacters = "";
    const charSet = new Set();
  
    for (const char of inputString) {
      if (!charSet.has(char)) {
        uniqueCharacters += char;
        charSet.add(char);
      }
    }
  
    return uniqueCharacters;
  }
console.log(removeDuplicates("djdnns"))
```
---

####  Reverse the words in a sentence.
```
function reverseWord(str){
  return str.split(" ").reverse().join(" ")
}
console.log("i am dhanu")
console.log(reverseWord("i am dhanu"))
```
---

####  Find the common characters between two strings.
```
function commonChar(str1, str2) {
  let commonChars = [];
  
  for (let char of str1) {
    if (str2.includes(char) && !commonChars.includes(char)) {
      commonChars.push(char);
    }
  }
  
  return commonChars.join('');
}

console.log(commonChar("ssjsj", "dhshdhb"));
```
---
#### Spcae before Capital Letter
```
function addSpacesWithoutPattern(inputString) {
  var outputString = "";
  
  for (var i = 0; i < inputString.length; i++) {
    var currentChar = inputString[i];
    
    if (currentChar === currentChar.toUpperCase() && i > 0) {
      outputString += " " + currentChar;
    } else {
      outputString += currentChar;
    }
  }
  
  return outputString;
}
var input = "MyNameIsJohn";
var output = addSpacesWithoutPattern(input);
console.log(output);
```

