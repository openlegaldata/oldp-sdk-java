
# CourtMinimal

## Properties
Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**id** | **Integer** |  |  [optional]
**name** | **String** | Full name of the court with location | 
**slug** | **String** | Type &amp; city name as lowercase | 
**city** | **Integer** | Court belongs to this city, if null court is state-level |  [optional]
**state** | **Integer** | Court belongs to this state (derive country of this field) | 
**jurisdiction** | **String** | Jurisdiction of court (ordinary, civil, ...) |  [optional]
**levelOfAppeal** | **String** | Subject-matter jurisdiction (local, federal, high court, ...) |  [optional]



