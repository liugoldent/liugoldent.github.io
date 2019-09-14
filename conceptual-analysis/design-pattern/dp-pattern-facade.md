# Facade（表象模式）

資料來源：

* [阿洲的程式教學：表象模式](http://monkeycoding.com/?p=975) 
* [Alex：JS\_Next（線上不公開課程）](https://www.youtube.com/user/achen224)

## Purpose

* 提供一個統一的介面，用來存取次系統的一群介面，讓次系統容易使用

## Conceptual

* 假設你今天要蛋炒飯，其步驟 
  * 放油 
  * 煎蛋 
  * 放飯＋醬油 
  * 把蛋和飯炒在一起 
* 假設你今天是一個客人，我只需要吃到蛋炒飯就好，我不用知道那麼多 
* 所以我_**只要知道原料**_（油、蛋、醬油、飯）就可以，丟進去後，_**機器自動**_煮。

## Code

```javascript
const tomato = function() {
  return "番茄";
};
const egg = function() {
  return "炒蛋";
};

const tomatoEgg = function() {
  return tomato() + egg();
};
console.log(tomato() + egg());
console.log(tomatoEgg());

//以上，使用者只要知道tomato / egg 即可，不用知道那是怎麼排列的
```














