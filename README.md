# Country Travel Information

[![Build Status](https://drone-io.tiepy.dev/api/badges/xgis-earth/action-query-country-travel-info/status.svg)](https://drone-io.tiepy.dev/xgis-earth/action-query-country-travel-info)

Hasura query action handler for reading country travel information.

## Development Environment

### Run Example

```bash
uvicorn main:app --reload --no-use-colors
```

## Deployment Configuration

### Action Definition

#### Query

```graphql
type Query {
  country_travel_info (
    country_code: String!
  ): TravelInfo!
}
```

#### New Types

```graphql
type TravelInfo {
  info: String!
  restrictions: String!
  sources: String!
  published: timestamptz!
}
```

#### Handler

http://query-country-travel-info/info
