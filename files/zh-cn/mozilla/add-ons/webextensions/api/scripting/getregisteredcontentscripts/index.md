---
title: scripting.getRegisteredContentScripts()
slug: Mozilla/Add-ons/WebExtensions/API/scripting/getRegisteredContentScripts
l10n:
  sourceCommit: b8a0743ca8b1e1b1b1a95cc93a4413c020f11262
---

{{AddonSidebar}}

返回所有使用 {{WebExtAPIRef("scripting.registerContentScripts()")}} 注册的脚本，或使用一个过滤器以获取已注册的一部分脚本。

> [!NOTE]
> 该方法在 Chrome 和 Firefox 101 的 Manifest V3 或更高版本中可用。在 Firefox 102+ 中，你也可以在 Manifest V2 中使用该方法。

要使用该方法，你必须取得 `"scripting"` [权限](/zh-CN/docs/Mozilla/Add-ons/WebExtensions/manifest.json/permissions)以及页面的 URL 权限，可以是明确的[主机权限](/zh-CN/docs/Mozilla/Add-ons/WebExtensions/manifest.json/permissions#主机权限)，也可以使用 [activeTab 权限](/zh-CN/docs/Mozilla/Add-ons/WebExtensions/manifest.json/permissions#活动标签权限)。

这是一个返回 [`Promise`](/zh-CN/docs/Web/JavaScript/Reference/Global_Objects/Promise) 的异步函数。

## 语法

```js-nolint
let scripts = await browser.scripting.getRegisteredContentScripts(
  filter          // 对象
)
```

### 参数

- `filter` {{optional_inline}}
  - : {{WebExtAPIRef("scripting.ContentScriptFilter")}}。用于过滤返回的注册脚本信息的过滤器。

### 返回值

[`Promise`](/zh-CN/docs/Web/JavaScript/Reference/Global_Objects/Promise)，以 {{WebExtAPIRef("scripting.RegisteredContentScript")}} 数组兑现。如果出现了错误，则该 promise 会被拒绝。

## 示例

该示例返回所有已注册的内容脚本：

```js
// 注册两个内容脚本
await browser.scripting.registerContentScripts([
  {
    id: "script-1",
    js: ["script-1.js"],
    matches: ["*://example.com/*"],
  },
  {
    id: "script-2",
    js: ["script-2.js"],
    matches: ["*://example.com/*"],
  },
]);

// 获取所有内容脚本
let scripts = await browser.scripting.getRegisteredContentScripts();
console.log(scripts.map((script) => script.id)); // ["script-1", "script-2"]

// 只返回第二个内容脚本
scripts = await browser.scripting.getRegisteredContentScripts({
  ids: ["script-2"],
});
console.log(scripts.map((script) => script.id)); // ["script-2"]
```

{{WebExtExamples}}

## 浏览器兼容性

{{Compat}}

> [!NOTE]
> 此 API 基于 Chromium 的 [`chrome.scripting`](https://developer.chrome.google.cn/docs/extensions/reference/api/scripting#method-getRegisteredContentScripts) API。
