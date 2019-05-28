+++
title = "Алгоритмы на JavaScript: пузырьковая сортировка"
date = 2017-05-28
+++

```js
const bubbleSort = (arr) => {
    for(let i = 0; i < arr.length - 1; i++) {
        for (let j = 0; j < arr.length - 1 ; j++) {
            if (arr[j] > arr[j + 1]) {
                let swap = arr[j];
                arr[j] = arr[j + 1];
                arr[j + 1] = swap;
            }
        }
    }
    return arr;
}

bubbleSort([37, 45, 29, 8, -3, 14]);
```
