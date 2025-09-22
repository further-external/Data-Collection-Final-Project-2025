# Internal Click

## Javascript Code
```js

window.dataLayer = window.dataLayer || [];
dataLayer.push({click_data: null}) // Clear the previous click_data object.
dataLayer.push({
  "event": "internalClick",
  "detailed_event": "Internal Click",
  "click_data": {
    "link_url": "<link_url>",
    "link_text": "<link_text>"
  }
});
```

| Path                   | Type   | Description                           | Example                                                              | Pattern | Min Length | Max Length | Minimum | Maximum | Multiple Of |
| ---------------------- | ------ | ------------------------------------- | -------------------------------------------------------------------- | ------- | ---------- | ---------- | ------- | ------- | ----------- |
| click\_data.link\_url  | string | Destination URL clicked (same domain) | [https://further-analytics.com/products](https://further-analytics.com/products) |         |            |            |         |         |             |
| click\_data.link\_text | string | Text label of the link (if present)   | Product Page                                                         |         |            |            |         |         |             |

