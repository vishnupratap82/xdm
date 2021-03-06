
# Time-series Schema Schema

```
https://ns.adobe.com/xdm/data/time-series
```

Used to indicate the behavior of time partitioned semantics when composed into data schemas.

| [Abstract](../../abstract.md) | [Extensible](../../extensions.md) | [Status](../../status.md) | [Identifiable](../../id.md) | [Custom Properties](../../extensions.md) | [Additional Properties](../../extensions.md) | Defined In |
|-------------------------------|-----------------------------------|---------------------------|-----------------------------|------------------------------------------|----------------------------------------------|------------|
| Can be instantiated | Yes | Stable | No | Forbidden | Permitted | [behaviors/time-series.schema.json](behaviors/time-series.schema.json) |
## Schema Hierarchy

* Time-series Schema `https://ns.adobe.com/xdm/data/time-series`
  * [Extensibility base schema](../datatypes/extensible.schema.md) `https://ns.adobe.com/xdm/common/extensible`


## Time-series Schema Example
```json
{
  "@id": "https://data.adobe.io/experienceid-123456",
  "xdm:timestamp": "2017-09-26T15:52:25+00:00",
  "xdm:eventType": "advertising.impressions"
}
```

# Time-series Schema Properties

| Property | Type | Required | Defined by |
|----------|------|----------|------------|
| [@id](#id) | `string` | Optional | Time-series Schema (this schema) |
| [xdm:eventType](#xdmeventtype) | `string` | Optional | Time-series Schema (this schema) |
| [xdm:timestamp](#xdmtimestamp) | `string` | Optional | Time-series Schema (this schema) |
| `*` | any | Additional | this schema *allows* additional properties |

## @id
### Identifier

A unique identifier for the time-series event.

`@id`
* is optional
* type: `string`
* defined in this schema

### @id Type


`string`
* format: `uri-reference` – URI Reference (according to [RFC3986](https://tools.ietf.org/html/rfc3986))






## xdm:eventType
### Event Type

The primary event type for this time-series record.

`xdm:eventType`
* is optional
* type: `string`
* defined in this schema

### xdm:eventType Type


`string`



### xdm:eventType Known Values
| Value | Description |
|-------|-------------|
| `advertising.completes` | Advertising Completes |
| `advertising.timePlayed` | Advertising Time Played |
| `advertising.federated` | Advertising Federated |
| `advertising.clicks` | Advertising Clicks |
| `advertising.conversions` | Advertising Conversions |
| `advertising.firstQuartiles` | Advertising First Quartiles |
| `advertising.impressions` | Advertising Impressions |
| `advertising.midpoints` | Advertising Midpoints |
| `advertising.starts` | Advertising Starts |
| `advertising.thirdQuartiles` | Advertising Third Quartiles |
| `web.webpagedetails.pageViews` | Web Webpagedetails Page Views |
| `web.webinteraction.linkClicks` | Web Webinteraction Link Clicks |
| `commerce.checkouts` | Commerce Checkouts |
| `commerce.productListAdds` | Commerce Product List Adds |
| `commerce.productListOpens` | Commerce Product List Opens |
| `commerce.productListRemovals` | Commerce Product List Removals |
| `commerce.productListReopens` | Commerce Product List Reopens |
| `commerce.productListViews` | Commerce Product List Views |
| `commerce.productViews` | Commerce Product Views |
| `commerce.purchases` | Commerce Purchases |
| `commerce.saveForLaters` | Commerce Save For Laters |
| `delivery.feedback` | Delivery Feedback |
| `message.feedback` | Message Feedback |
| `message.tracking` | Message Tracking |




## xdm:timestamp
### Timestamp

The time when an event or observation occurred.

`xdm:timestamp`
* is optional
* type: `string`
* defined in this schema

### xdm:timestamp Type


`string`
* format: `date-time` – date and time (according to [RFC 3339, section 5.6](http://tools.ietf.org/html/rfc3339))





