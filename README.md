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

```

### Console以外の動き（もしあれば）

【ここに書く（なければ省略可）】

### 分かったこと

【ここに書く】

### 疑問・分からないこと（もしあれば）

【ここに書く（なければ省略可）】
