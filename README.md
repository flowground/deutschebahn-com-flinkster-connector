# ![LOGO](logo.png) Flinkster_API_NG **flow**ground Connector

## Description

A generated **flow**ground connector for the Flinkster_API_NG API (version v1).

Generated from: https://api.apis.guru/v2/specs/deutschebahn.com/flinkster/v1/swagger.json<br/>
Generated at: 2019-05-07T17:40:13+03:00

## API Description

This REST-API enables you to query for private transport sharing offers provided by companies and cities in Germany, Netherland and Austria. 
You can search for informations about the rental stations (points or areas) where you can find the rentals by utilizing the /areas/ ressource. 
With the help of the proximity search in the /bookingproposals/ URI you can request the availabilities of the rentalobjects for spontaneous or planed usage in the future. 

Feel free to browse through data by setting the parameter 'providernetwork' to the value: 
 1: Search for car sharing offers provided by the Flinkster platform (http://www.flinkster.de)
2: Finding bike rental offers from Call a Bike (http://www.callabike.de) 

You can find more details in the documentation section (Unfortunately only available in german language).

Have lots of fun and we are lucky to take notice of your products or getting your feedback.

## Authorization

This API does not require authorization.

## Actions

### List Areas by Criteria.

> Search for areas (locations of rental objects) by criteria.

*Tags:* `areas`

#### Input Parameters
* `lat` - _optional_
* `lon` - _optional_
* `radius` - _optional_
* `offset` - _optional_
* `limit` - _optional_
* `expand` - _optional_
* `type` - _optional_
* `provider` - _optional_
* `providernetwork` - _optional_

### Get area by UID.

> Search for a specific area by UID.

*Tags:* `areas`

#### Input Parameters
* `areaUID` - _required_ - The Area UID 
* `expand` - _optional_ - Expand Provider

### Query for available RentalObjects of a specific view

> Here you can query all bookable Rental Objects with different Parameters (Time, Location,...)

*Tags:* `bookingproposals`

#### Input Parameters
* `lat` - _optional_
* `lon` - _optional_
* `radius` - _optional_
* `offset` - _optional_
* `limit` - _optional_
* `providernetwork` - _optional_
* `begin` - _optional_
* `end` - _optional_
* `expand` - _optional_
* `view` - _optional_

### Show index.

> Show Service index.

*Tags:* `index`

### Lists all categories

> Search for categorie.

*Tags:* `categories`

#### Input Parameters
* `providernetworkUID` - _required_
* `expand` - _optional_

### Get a Category by UID

> Search for categorie.

*Tags:* `categories`

#### Input Parameters
* `providernetworkUID` - _required_ - Provider Network UID
* `categoryUID` - _required_
* `expand` - _optional_

### Get information about the prices.

> Prices of a rental object by query params. The params depend on the price determination strategy of the provider network.

*Tags:* `prices`

#### Input Parameters
* `providernetworkUID` - _required_

### Get information about the RentalObject.

> Get information about the Rental Object.

*Tags:* `rentalobjects`

#### Input Parameters
* `rentalObjectUID` - _required_
* `providernetworkUID` - _required_
* `expand` - _optional_

### Get information about the ProviderNetworkResources.

> Get information about the ProviderNetworkResources.

*Tags:* `providernetworks`

#### Input Parameters
* `uid` - _required_

### Get information about the ProviderResourceImpl.

> Get information about the ProviderResourcesCtrl.

*Tags:* `providers`

#### Input Parameters
* `uid` - _required_

## License

**flow**ground :- Telekom iPaaS / deutschebahn-com-flinkster-connector<br/>
Copyright © 2019, [Deutsche Telekom AG](https://www.telekom.de)<br/>
contact: flowground@telekom.de

All files of this connector are licensed under the Apache 2.0 License. For details
see the file LICENSE on the toplevel directory.
