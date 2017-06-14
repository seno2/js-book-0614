# 6/14 課題 学んだ記録

自身が学んだ記録を作りましょう。

- 関数(`function` で始まるコード)は全て function.js に書きます
- その他をREADME.md（このファイル）に書いていきます
    - 書き方は README-example.md (同じフォルダに同梱) を参考にしてください
- 書き方は自身でアレンジしてもかまいません


--------------------------------------

## 授業スライドの説明（4時間目～5時間目）

説明の中で実行したログ、分かったこと、疑問などがあればここに書く。

### Consoleの実行ログ

```
var sampleArray = [];
undefined
sampleArray;
[]
var sampleArray = [1,3,5];
undefined
sampleArray
(3) [1, 3, 5]
var sampleArray= [];
undefined
sampleArray.push(59)
1
sampleArray;
[59]
sampleArray.push(61);
2
sampleArray;
(2) [59, 61]
sampleArray[0];
59
sampleArray[1];
61
sampleArray[2];
undefined
sampleArray.splice(0,1);
[59]
sampleArray;
[61]
sampleArray.push(67);
2
sampleArray.push(71);
3
sampleArray.push(73);
4
sampleArray;
(4) [61, 67, 71, 73]
sampleArray.splice(1,2);
(2) [67, 71]
sampleArray;
(2) [61, 73]
sampleArray.length;
2
function calculateTaxIncluding(prices) {
  var results = [];
 for (var index = 0, length = prices.length; index < length; index++)
 {
results.push(prices[index] * 1.08);
 }
return results;
}
undefined
calculateTaxIncluding([100,200,40,50]);
(4) [108, 216, 43.2, 54]
var a =[0, 1, 1, 2, 3, 5, 8];
undefined
a.tostring();
VM703:1 Uncaught TypeError: a.tostring is not a function
    at <anonymous>:1:3
(anonymous) @ VM703:1
a.toString();
"0,1,1,2,3,5,8"
var a = [0,1,1,2,3,5,8];
undefined
a.join(' and ');
"0 and 1 and 1 and 2 and 3 and 5 and 8"
var a =1[0,1,1,2,3,5,8]
undefined
a.join();
VM768:1 Uncaught TypeError: Cannot read property 'join' of undefined
    at <anonymous>:1:2
(anonymous) @ VM768:1
var a = [0,1,1,2,3,5,8];
undefined
a.index0f(5);
VM817:1 Uncaught TypeError: a.index0f is not a function
    at <anonymous>:1:3
(anonymous) @ VM817:1
var a =[0,1,1,2,3,5,8];
undefined
a.indexf(4);
VM852:1 Uncaught TypeError: a.indexf is not a function
    at <anonymous>:1:3
(anonymous) @ VM852:1
var a = [0,1,1,2,3,5,8];
undefined
a.index0f(4);
VM962:1 Uncaught TypeError: a.index0f is not a function
    at <anonymous>:1:3
(anonymous) @ VM962:1
vara = [0,1,1,2,3,5,8];
(7) [0, 1, 1, 2, 3, 5, 8]
var a = [0,1,1,2,3,5,8];
undefined
a.index0f(1);
VM1003:1 Uncaught TypeError: a.index0f is not a function
    at <anonymous>:1:3
(anonymous) @ VM1003:1
var a = [0,1,1,2,3,5,8];
undefined
a.lastIndex0f(1);
VM1074:1 Uncaught TypeError: a.lastIndex0f is not a function
    at <anonymous>:1:3
(anonymous) @ VM1074:1
```

### Console以外の動き（もしあれば）

【ここに書く（なければ省略可）】

### 分かったこと

配列の作り方

### 疑問・分からないこと（もしあれば）

「要素が存在するか確認する」でa.index0fを行っても記載通りの結果にならなかった。

--------------------------------------

以下、教科書の自分で読んだ・実行した箇所について書く。

## 4-x ○○ (p.xx)

### Consoleの実行ログ

```
var sampleHashMap = {};
undefined
sampleHashMap['test']
undefined
sampleHashMap['test'] = 5;
5
sampleHashMap['test'];
5
sampleHashMap.test;
5
sampleHashMap.test; = 7;
VM1190:1 Uncaught SyntaxError: Unexpected token =
sampleHashMap.test = 7;
7
sampleHashMap.test;
7
var sampleHashMap ={ test : 11};
undefined
sampleHashMap.test;
11
function sumInformationScore(scores) {
var toatal =0;
for (var index = 0; index < scores.length; index++) {
  total += scores[index].information;
}
  return total;
}

function sumEnglishScore(scores) {
  var total = 0;
  for (var index = 0; index < scores.length; index++) {
    total += scores[index].english;
  }
  return total;
}
undefined
function sampleFunction(message = 'test') {return message };
undefined
var functionVar = sampleFunction;
undefined
functionVar();
"test"
functionVar('hoge');
"hoge"
functionVar;
function sampleFunction(message = 'test') {return message }
function callTarget(target) {return target(); };
undefined
function returnSomeString() { return 'Sample'; };
undefined
function returnSomeFunction() {return returnSomeString; };
undefined
callTarget(returnSomeString);
"Sample"
returnSomeFunction();
function returnSomeString() { return 'Sample'; }
returnSomeFunction()();
"Sample"
function getInformationScore(score) {
  return score.information;
}

function getEnglishScore(score) {
   return score.english;
}

function calculateTotal(scores, getTarget) {
  var total =0;
  for (var index = 0; index < scores.length; index++) {
total += getTarget(scores[index]);
  }

return total;
}
undefined
calculateTotal(examinationScores, getInfomationScore;
VM2796:1 Uncaught SyntaxError: missing ) after argument list
calculateTotal(examinationScores, getInfomationScore);
VM2800:1 Uncaught ReferenceError: examinationScores is not defined
    at <anonymous>:1:16
(anonymous) @ VM2800:1
calculateTotal(examinationScores, getInformationScore;
VM3099:1 Uncaught SyntaxError: missing ) after argument list
calculateTotal(examinationScores, getInformationScore);
VM3102:1 Uncaught ReferenceError: examinationScores is not defined
    at <anonymous>:1:16
(anonymous) @ VM3102:1
function getInformationScore(score) {
  return score.information;
}

function getEnglishScore(score) {
   return score.english;
}

function calculateTotal(scores, getTarget) {
  var total =0;
  for (var index = 0; index < scores.length; index++) {
total += getTarget(scores[index]);
  }

return total;
}
undefined
calculateTotal(examinationScores, getInformationScore);
VM3105:1 Uncaught ReferenceError: examinationScores is not defined
    at <anonymous>:1:16
(anonymous) @ VM3105:1
sumInformationScore(examinationScores);
VM3183:1 Uncaught ReferenceError: examinationScores is not defined
    at <anonymous>:1:21
(anonymous) @ VM3183:1
var functionExpression =
  functin getInformationScore(score) {
    return score.information;
  };
VM3293:2 Uncaught SyntaxError: Unexpected identifier
var functionExpression =
  function getInformationScore(score) {
    return score.information;
  };
undefined
functionExpression;
function getInformationScore(score) {
    return score.information;
  }
getInformationScore(score)
VM3387:1 Uncaught ReferenceError: score is not defined
    at <anonymous>:1:21
(anonymous) @ VM3387:1
getInformationScore;
function getInformationScore(score) {
  return score.information;
}
calculateTotal(examinationScores, functionExpression);
VM3539:1 Uncaught ReferenceError: examinationScores is not defined
    at <anonymous>:1:16
(anonymous) @ VM3539:1
calculateTotal(examinationScores,
  function getInformationScore(score) {
     return score.information;
}};
VM3631:4 Uncaught SyntaxError: missing ) after argument list
calculateTotal(examinationScores,
  function(score) {
    return score.information;
}};
VM3753:4 Uncaught SyntaxError: missing ) after argument list
calculateTotal(examinationScores,
  function(score) {
    return score.information;
});
VM3758:1 Uncaught ReferenceError: examinationScores is not defined
    at <anonymous>:1:16
(anonymous) @ VM3758:1
calculateTotal(examinationScores,
   (score) => {
     return score. information;
});
VM3879:1 Uncaught ReferenceError: examinationScores is not defined
    at <anonymous>:1:16
(anonymous) @ VM3879:1
calculateTotal(examinationScores,
   score => {
     return score. information;
});
VM3935:1 Uncaught ReferenceError: examinationScores is not defined
    at <anonymous>:1:16
(anonymous) @ VM3935:1
calculateTotal(examinationScores, score => score.information);
VM4037:1 Uncaught ReferenceError: examinationScores is not defined
    at <anonymous>:1:16
(anonymous) @ VM4037:1
var functionVar1 = () => '1st';
undefined
functionVar1();
"1st"
functionVar1 = () => '2nd';
() => '2nd'
functionVar1();
"2nd"
var functionVar1 = function function1() { console.log(function1); };
undefined
functionVar1();
VM4205:1 function function1() { console.log(function1); }
undefined
console.log(function1);
VM4277:1 Uncaught ReferenceError: function1 is not defined
    at <anonymous>:1:13
(anonymous) @ VM4277:1
function function1() { return '1st'; };
undefined
var function2= function1;
undefined
function1 = function function2() { return '2nd'; };
function function2() { return '2nd'; }
function1();
"2nd"
function2();
"1st"
function3();
VM4471:1 Uncaught ReferenceError: function3 is not defined
    at <anonymous>:1:1
(anonymous) @ VM4471:1
function3();
function function3() {return '3rd'; };
"3rd"
var functionVar4;
functionVar4();
functionvar4 = () => console.log('3rd');
VM4597:2 Uncaught TypeError: functionVar4 is not a function
    at <anonymous>:2:1
(anonymous) @ VM4597:2
```

### Console以外の動き（もしあれば）

【ここに書く（なければ省略可）】

### 分かったこと

配列と関数について

### 疑問・分からないこと（もしあれば）

calculateがうまくできなかった
