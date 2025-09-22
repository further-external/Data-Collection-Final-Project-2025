# Outbound Click

## Javascript Code
```js

window.dataLayer = window.dataLayer || [];
dataLayer.push({click_data: null}) // Clear the previous click_data object.
dataLayer.push({
  "event": "outboundClick",
  "detailed_event": "Outbound Click",
  "click_data": {
    "link_url": "<link_url>",
    "link_text": "<link_text>"
  }
});
```

| Path                   | Type   | Description                               | Example                                                              | Pattern | Min Length | Max Length | Minimum | Maximum | Multiple Of |
| ---------------------- | ------ | ----------------------------------------- | -------------------------------------------------------------------- | ------- | ---------- | ---------- | ------- | ------- | ----------- |
| click\_data.link\_url  | string | Destination URL clicked (external domain) | [https://www.youtube.com/@Further_Worldwide](https://www.youtube.com/@Further_Worldwide) |         |            |            |         |         |             |
| click\_data.link\_text | string | Text label of the link (if present)       | Watch on YouTube                                                     |         |            |            |         |         |             |
