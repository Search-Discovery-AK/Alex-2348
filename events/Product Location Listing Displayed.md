# Product Location Listing Displayed

### This event is part of the page load sequence, including virtual page loads in the case of single page apps, and must be pushed between the `Page Load Started` and `Page Load Completed` events.

## Javascript Code
```js
window.appEventData = window.appEventData || [];
appEventData.push({
  "event": "Product Location Listing Displayed",
    "listingDisplayed": {
        "listing": [
            {
                "isDisplayed": "<isDisplayed>",
                "location": {
                    "locationId": "<locationId>"
                }
            }
        ],
        "listingDriver": "<listingDriver>",
        "listingType": "<listingType>"
    }
});
```

## Variable Definitions

|Field|Type|Description|Example|Pattern|Min Length|Max Length|Minimum|Maximum|Multiple Of|
| --- | --- | --- | --- | --- | --- | --- | --- | --- | --- |
|isDisplayed|boolean|Helper node used by AA Product String Builder to set product scoped events|true|||||||
|listingDriver|string|Describes the action that caused the listing to be displayed|Onsite Search, Curated Assortment, Navigation|||||||
|listingType|string|The type of results being listed|text, product, location, event, room, product location|||||||
|locationId|string|Unique Identifier of a Location. |155, 65588, 987764448|||||||
