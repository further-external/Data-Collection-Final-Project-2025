## Javascript Code
```js
window.dataLayer = window.dataLayer || [];
dataLayer.push({page_data: null}) // Clear the previous page_data object.
dataLayer.push({
  "event": "pageView",
  "detailed_event": "Page View",
  "page_data": {
    "page_url": "<page_url>"
    "page_path": "page_path",
    "page_title": "page_title"
  }
});
```
| Path                   | Type   | Description                              | Example                                                                | Pattern | Min Length | Max Length | Minimum | Maximum | Multiple Of |
| ---------------------- | ------ | ---------------------------------------- | ---------------------------------------------------------------------- | ------- | ---------- | ---------- | ------- | ------- | ----------- |
| page\_data.page\_url   | string | Full URL of the page                     | https://further-analytics.com |         |            |            |         |         |             |
| page\_data.page\_path  | string | Path portion of the page URL             | /products                                                              |         |            |            |         |         |             |
| page\_data.page\_title | string | Title of the page currently being viewed | Our Products                                                           |         |            |            |         |         |             |
