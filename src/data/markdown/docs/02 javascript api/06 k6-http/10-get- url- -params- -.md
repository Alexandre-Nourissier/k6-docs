---
title: "get( url, [params] )"
description: "Issue an HTTP GET request."
---

Make a GET request.

| Parameter         | Type   | Description                                                                                           |
| ----------------- | ------ | ----------------------------------------------------------------------------------------------------- |
| url               | string | Request URL (e.g. `http://example.com`).                                                              |
| params (optional) | object | [Params](/javascript-api/k6-http/params-k6-http) object containing additional request parameters. |

### Returns

| Type     | Description |
| -------- | ----------- |
| [Response](/javascript-api/k6-http/response-k6-http) | HTTP Response object. |


### Example fetching a URL

<div class="code-group" data-props='{"labels": []}'>

```js
import http from 'k6/http';

export default function() {
  let res = http.get('https://k6.io');
}
```

</div>
