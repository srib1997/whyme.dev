---
title: "React hooks"
date: "2019-03-12T10:00:00+08:00"
description: "Hook 是React 16.8中的新增功能。 它們允許您在不編寫 class 的情況下使用 state 和其他 React 功能。"
authors:
  - name: Srib Chao
    avatar: /team/srib.jpg
---

# React Hooks 

---

```js
import React, { useState } from 'react';

function Example() {
  // Declare a new state variable, which we'll call "count"
  // 聲明一個新的狀態變量，我們將其稱為 “count”
  const [count, setCount] = useState(0);

  return (
    <div>
      <p>You clicked {count} times</p>
      <button onClick={() => setCount(count + 1)}>
        Click me
      </button>
    </div>
  );
}
```

這個新函數 useState 是我們將要學習的第一個 “hook”，但這個例子只是一個測試。 如果它沒有意義，請不要擔心！

**你可以在下一頁開始學習**[Hooks](https://reactjs.org/docs/hooks-overview.html)。 在這個頁面上，我們將繼續解釋為什麼我們將 Hook 添加到 React 以及它們如何幫助您編寫出色的應用程序。

---

```
注意

React 16.8.0是第一個支持Hooks的版本。 升級時，不要忘記更新所有包，包括React DOM。 

React Native將在下一個穩定版本中支持Hook。
```

---

視頻介紹

在React Conf 2018中，Sophie Alpert和Dan Abramov介紹了Hooks，隨後Ryan Florence演示瞭如何重構應用程序以使用它們。 

觀看視頻：

<iframe width="560" height="315" src="https://www.youtube.com/embed/dpw9EHDh2bM" frameborder="0" allow="accelerometer; autoplay; encrypted-media; gyroscope; picture-in-picture" allowfullscreen></iframe>

---

## 沒有重大變化

在我們繼續之前，請注意Hooks是：

**完全自己選擇加入**。 您可以在幾個 components 中嘗試 Hooks，而無需重寫任何現有代碼。 但是如果你不想，你現在不必學習或使用Hooks。

**100％向後兼容**。  Hook 不包含任何重大更改。

**現在可以使用**。 v16.8.0的發布，現在可以使用 Hook。

**沒有計劃從 React 中刪除 class**。 您可以在本頁底部閱讀有關 Hooks 逐步採用策略的更多信息。

**hook 不會取代你對 React 概念的了解**。 相反，Hooks為您已經知道的 React 概念提供了更直接的API：
props，state，context，refs和lifecycle。 
正如我們稍後將展示的那樣，Hooks 還提供了一種新的強大方式來組合它們。