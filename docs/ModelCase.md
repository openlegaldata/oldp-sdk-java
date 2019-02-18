
# ModelCase

## Properties
Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**id** | **Integer** |  |  [optional]
**slug** | **String** |  |  [optional]
**court** | [**CourtMinimal**](CourtMinimal.md) |  |  [optional]
**fileNumber** | **String** | File number as defined by court | 
**date** | [**LocalDate**](LocalDate.md) | Publication date as in source |  [optional]
**createdDate** | [**OffsetDateTime**](OffsetDateTime.md) | Entry is created at this date time |  [optional]
**updatedDate** | [**OffsetDateTime**](OffsetDateTime.md) | Date time of last change |  [optional]
**type** | **String** | Type of decision (Urteil, Beschluss, ...) |  [optional]
**ecli** | **String** | European Case Law Identifier |  [optional]
**content** | **String** | Case full-text formatted in Legal HTML | 



