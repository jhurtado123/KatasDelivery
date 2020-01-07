# KatasDelivery

##Numbers to letters

function switcher(x){
  let relation = {29: ' ', 28: '?', 27: '!', 26: 'a', 25: 'b', 24: 'c', 23:'d',22:'e',21:'f',20:'g',19:'h',18:'i',17:'j',16:'k',15:'l',14:'m',13:'n',12:'o',11:'p',10:'q',9:'r',8:'s',7:'t',6:'u',5:'v',4:'w',3:'x',2:'y',1:'z'};
   
  return x.reduce((a, val) => a + relation[parseInt(val)], "");
}


##Remove first and last character

function removeChar(str){
 //You got this!
  return str.substring(1, str.length-1);
};

##VOWEL COUNT 

function getCount(str) {
   return str.match(/[aeiou]/g) ? str.match(/[aeiou]/g).length : 0 ;
}

##SUM MIXED ARRAYS

function sumMix(x){
  return x.reduce( (a,val) => a + parseInt(val), 0);
}


##COUNT OF POSITIVES

function countPositivesSumNegatives(input) {
  if (input == null || input.length == 0) return [];
  let sum = 0;
   input.forEach((a) => { if (a < 0) sum += a });
  return [input.filter(a => a > 0).length,sum ];
}

##GET THE MEAN OF AN ARRAY

function getAverage(marks){
  return parseInt(marks.reduce((a,b) => a+b) / marks.length);
}

##Find numbers which are divisible by given number

function divisibleBy(numbers, divisor){
  return numbers.filter((a) => a % divisor == 0);
}


##LIST FILTERING 

function filter_list(l) {
  // Return a new array with the strings filtered out
  return l.filter((a) => typeof a == 'number');
}

##CREDIT CARD MASK

// return masked string
function maskify(cc) {
    let string = "";
    for (let i = 0; i < cc.length; i++) {
      if (i < cc.length-4) {
        string += "#"; 
      } else {
        string += cc.charAt(i);
      }
      
    }
    return string;
}

##FLATTEN

##Square every digit

function squareDigits(num){
  //may the code be with you
  return parseInt(num.toString().split('').reduce((a, b) => a + Math.pow(b,2).toString(), ''));
}

```
