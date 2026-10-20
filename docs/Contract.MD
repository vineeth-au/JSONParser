# Lookup behavior contract

This document defines the intended behavior of the existing `getNodeValue` method. Some cases
require changes to the current implementation.

## Example input

```json
{
  "vehicle": {
    "id": "V123",
    "nickname": null
  },
  "speeds": [
    50,
    72
  ]
}
```

## Expected behavior

Paths use the existing dot-separated syntax.

- `vehicle.id` -> Returns `String` "V123"
- `vehicle.nickname` -> Returns `JSONObject.NULL`