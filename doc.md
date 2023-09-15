# Protocol Documentation
<a name="top"></a>

## Table of Contents

- [shopping.proto](#shopping-proto)
    - [AddItemRequest](#shoppingcart-v1-AddItemRequest)
    - [AddItemResponse](#shoppingcart-v1-AddItemResponse)
  
    - [ShoppingCartService](#shoppingcart-v1-ShoppingCartService)
  
- [Scalar Value Types](#scalar-value-types)



<a name="shopping-proto"></a>
<p align="right"><a href="#top">Top</a></p>

## shopping.proto



<a name="shoppingcart-v1-AddItemRequest"></a>

### AddItemRequest



| Field | Type | Label | Description |
| ----- | ---- | ----- | ----------- |
| product_id | [string](#string) |  | 商品ID: JANコード |
| quantity | [int32](#int32) |  | 個数 |






<a name="shoppingcart-v1-AddItemResponse"></a>

### AddItemResponse



| Field | Type | Label | Description |
| ----- | ---- | ----- | ----------- |
| success | [bool](#bool) |  | 成功かどうかのフラグ |
| total_price | [int32](#int32) |  | 合計金額 |





 

 

 


<a name="shoppingcart-v1-ShoppingCartService"></a>

### ShoppingCartService
ショッピングカートサービスです。

| Method Name | Request Type | Response Type | Description |
| ----------- | ------------ | ------------- | ------------|
| AddItem | [AddItemRequest](#shoppingcart-v1-AddItemRequest) | [AddItemResponse](#shoppingcart-v1-AddItemResponse) | ショッピングカートに商品を追加します。同じ商品が追加された場合には個数が合計されます。 |

 



## Scalar Value Types

| .proto Type | Notes | C++ | Java | Python | Go | C# | PHP | Ruby |
| ----------- | ----- | --- | ---- | ------ | -- | -- | --- | ---- |
| <a name="double" /> double |  | double | double | float | float64 | double | float | Float |
| <a name="float" /> float |  | float | float | float | float32 | float | float | Float |
| <a name="int32" /> int32 | Uses variable-length encoding. Inefficient for encoding negative numbers – if your field is likely to have negative values, use sint32 instead. | int32 | int | int | int32 | int | integer | Bignum or Fixnum (as required) |
| <a name="int64" /> int64 | Uses variable-length encoding. Inefficient for encoding negative numbers – if your field is likely to have negative values, use sint64 instead. | int64 | long | int/long | int64 | long | integer/string | Bignum |
| <a name="uint32" /> uint32 | Uses variable-length encoding. | uint32 | int | int/long | uint32 | uint | integer | Bignum or Fixnum (as required) |
| <a name="uint64" /> uint64 | Uses variable-length encoding. | uint64 | long | int/long | uint64 | ulong | integer/string | Bignum or Fixnum (as required) |
| <a name="sint32" /> sint32 | Uses variable-length encoding. Signed int value. These more efficiently encode negative numbers than regular int32s. | int32 | int | int | int32 | int | integer | Bignum or Fixnum (as required) |
| <a name="sint64" /> sint64 | Uses variable-length encoding. Signed int value. These more efficiently encode negative numbers than regular int64s. | int64 | long | int/long | int64 | long | integer/string | Bignum |
| <a name="fixed32" /> fixed32 | Always four bytes. More efficient than uint32 if values are often greater than 2^28. | uint32 | int | int | uint32 | uint | integer | Bignum or Fixnum (as required) |
| <a name="fixed64" /> fixed64 | Always eight bytes. More efficient than uint64 if values are often greater than 2^56. | uint64 | long | int/long | uint64 | ulong | integer/string | Bignum |
| <a name="sfixed32" /> sfixed32 | Always four bytes. | int32 | int | int | int32 | int | integer | Bignum or Fixnum (as required) |
| <a name="sfixed64" /> sfixed64 | Always eight bytes. | int64 | long | int/long | int64 | long | integer/string | Bignum |
| <a name="bool" /> bool |  | bool | boolean | boolean | bool | bool | boolean | TrueClass/FalseClass |
| <a name="string" /> string | A string must always contain UTF-8 encoded or 7-bit ASCII text. | string | String | str/unicode | string | string | string | String (UTF-8) |
| <a name="bytes" /> bytes | May contain any arbitrary sequence of bytes. | string | ByteString | str | []byte | ByteString | string | String (ASCII-8BIT) |

