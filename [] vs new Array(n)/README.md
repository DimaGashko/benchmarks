# [] vs new Array(n)

Иногда может понадобиться создавать (генерировать) большие массивы.
Как эффективнее это сделать? 

Вот два варианта: 

```javascript

function usually(n) {
   var arr = [];
   for (var i = 0; i < n; i++) {
      arr[i] = i;
   }
}

function constr(n) {
   var arr = new Array(n);

   for (var i = 0; i < n; i++) {
      arr[i] = i;
   }
}

```

Тест на jsperf.com: https://jsperf.com/writetobigarray/



