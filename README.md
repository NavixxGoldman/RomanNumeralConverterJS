# RomanNumeralConverterJS
Roman Numeral Converter  Convert the given number into a roman numeral.  All roman numerals will be provided in upper-case.
```javascript
function convertToRoman(num) {
    var romanArray=[
        "M","CM","D","CD","C","XC","L","XL","X","IX","V","IV","I"];
    var numeralArray=[1000,900,500,400,100,90,50,40,10,9,5,4,1];
     var romanized="";
     //Loops
 for (var index=0;index<numeralArray.length;index++){
     while (numeralArray[index] <= num){
            romanized += romanArray[index];
            num -=numeralArray[index];
     }
 }
   

 return romanized;
}

console.log(convertToRoman(6)) ;
console.log(convertToRoman(29)) ;
console.log(convertToRoman(3999));
```
