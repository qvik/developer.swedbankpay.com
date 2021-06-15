---
title: Server -
---
//[sdk](../../../../index)/[com.swedbankpay.mobilesdk.merchantbackend](../../index)/[MerchantBackendProblem](../index)/[Server](index)



# Server  
 [androidJvm] sealed class [Server](index) : [MerchantBackendProblem](../index)

Base class for [Problems](../index) caused by the service backend.



Any unexpected response where the HTTP status is outside 400-499 results in a Server Problem; usually it means the status was in 500-599.

   


## Types  
  
|  Name |  Summary | 
|---|---|
| <a name="com.swedbankpay.mobilesdk.merchantbackend/MerchantBackendProblem.Server.Companion///PointingToDeclaration/"></a>[Companion](-companion/index)| <a name="com.swedbankpay.mobilesdk.merchantbackend/MerchantBackendProblem.Server.Companion///PointingToDeclaration/"></a>[androidJvm]  <br>Content  <br>object [Companion](-companion/index)  <br><br><br>|
| <a name="com.swedbankpay.mobilesdk.merchantbackend/MerchantBackendProblem.Server.MobileSDK///PointingToDeclaration/"></a>[MobileSDK](-mobile-s-d-k/index)| <a name="com.swedbankpay.mobilesdk.merchantbackend/MerchantBackendProblem.Server.MobileSDK///PointingToDeclaration/"></a>[androidJvm]  <br>Content  <br>sealed class [MobileSDK](-mobile-s-d-k/index) : [MerchantBackendProblem.Server](index)  <br>More info  <br>Base class for [Server](index) Problems defined by the example backend.  <br><br><br>|
| <a name="com.swedbankpay.mobilesdk.merchantbackend/MerchantBackendProblem.Server.SwedbankPay///PointingToDeclaration/"></a>[SwedbankPay](-swedbank-pay/index)| <a name="com.swedbankpay.mobilesdk.merchantbackend/MerchantBackendProblem.Server.SwedbankPay///PointingToDeclaration/"></a>[androidJvm]  <br>Content  <br>sealed class [SwedbankPay](-swedbank-pay/index) : [MerchantBackendProblem.Server](index), [SwedbankPayProblem](../../-swedbank-pay-problem/index)  <br>More info  <br>Base class for [Server](index) problems defined by the Swedbank Pay backend.  <br><br><br>|
| <a name="com.swedbankpay.mobilesdk.merchantbackend/MerchantBackendProblem.Server.Unknown///PointingToDeclaration/"></a>[Unknown](-unknown/index)| <a name="com.swedbankpay.mobilesdk.merchantbackend/MerchantBackendProblem.Server.Unknown///PointingToDeclaration/"></a>[androidJvm]  <br>Content  <br>class [Unknown](-unknown/index)(**jsonObject**: JsonObject) : [MerchantBackendProblem.Server](index)  <br>More info  <br>[Server](index) problem with an unrecognized type.  <br><br><br>|


## Functions  
  
|  Name |  Summary | 
|---|---|
| <a name="android.os/Parcelable/describeContents/#/PointingToDeclaration/"></a>[describeContents](-unknown/index.md#-1578325224%2FFunctions%2F-1404661416)| <a name="android.os/Parcelable/describeContents/#/PointingToDeclaration/"></a>[androidJvm]  <br>Content  <br>abstract fun [describeContents](-unknown/index.md#-1578325224%2FFunctions%2F-1404661416)(): [Int](https://kotlinlang.org/api/latest/jvm/stdlib/kotlin/-int/index.html)  <br><br><br>|
| <a name="com.swedbankpay.mobilesdk/Problem/equals/#kotlin.Any?/PointingToDeclaration/"></a>[equals](../../../com.swedbankpay.mobilesdk/-problem/equals)| <a name="com.swedbankpay.mobilesdk/Problem/equals/#kotlin.Any?/PointingToDeclaration/"></a>[androidJvm]  <br>Content  <br>open operator override fun [equals](../../../com.swedbankpay.mobilesdk/-problem/equals)(other: [Any](https://kotlinlang.org/api/latest/jvm/stdlib/kotlin/-any/index.html)?): [Boolean](https://kotlinlang.org/api/latest/jvm/stdlib/kotlin/-boolean/index.html)  <br><br><br>|
| <a name="com.swedbankpay.mobilesdk/Problem/hashCode/#/PointingToDeclaration/"></a>[hashCode](../../../com.swedbankpay.mobilesdk/-problem/hash-code)| <a name="com.swedbankpay.mobilesdk/Problem/hashCode/#/PointingToDeclaration/"></a>[androidJvm]  <br>Content  <br>open override fun [hashCode](../../../com.swedbankpay.mobilesdk/-problem/hash-code)(): [Int](https://kotlinlang.org/api/latest/jvm/stdlib/kotlin/-int/index.html)  <br><br><br>|
| <a name="com.swedbankpay.mobilesdk/Problem/toString/#/PointingToDeclaration/"></a>[toString](../../../com.swedbankpay.mobilesdk/-problem/to-string)| <a name="com.swedbankpay.mobilesdk/Problem/toString/#/PointingToDeclaration/"></a>[androidJvm]  <br>Content  <br>open override fun [toString](../../../com.swedbankpay.mobilesdk/-problem/to-string)(): [String](https://kotlinlang.org/api/latest/jvm/stdlib/kotlin/-string/index.html)  <br><br><br>|
| <a name="com.swedbankpay.mobilesdk.merchantbackend/MerchantBackendProblem/writeToParcel/#android.os.Parcel#kotlin.Int/PointingToDeclaration/"></a>[writeToParcel](../write-to-parcel)| <a name="com.swedbankpay.mobilesdk.merchantbackend/MerchantBackendProblem/writeToParcel/#android.os.Parcel#kotlin.Int/PointingToDeclaration/"></a>[androidJvm]  <br>Content  <br>open override fun [writeToParcel](../write-to-parcel)(parcel: [Parcel](https://developer.android.com/reference/kotlin/android/os/Parcel.html), flags: [Int](https://kotlinlang.org/api/latest/jvm/stdlib/kotlin/-int/index.html))  <br><br><br>|


## Properties  
  
|  Name |  Summary | 
|---|---|
| <a name="com.swedbankpay.mobilesdk.merchantbackend/MerchantBackendProblem.Server/detail/#/PointingToDeclaration/"></a>[detail](index.md#-829000368%2FProperties%2F-1404661416)| <a name="com.swedbankpay.mobilesdk.merchantbackend/MerchantBackendProblem.Server/detail/#/PointingToDeclaration/"></a> [androidJvm] val [detail](index.md#-829000368%2FProperties%2F-1404661416): [String](https://kotlinlang.org/api/latest/jvm/stdlib/kotlin/-string/index.html)?RFC 7807 default property: a detailed explanation of the problem   <br>|
| <a name="com.swedbankpay.mobilesdk.merchantbackend/MerchantBackendProblem.Server/instance/#/PointingToDeclaration/"></a>[instance](index.md#1295215756%2FProperties%2F-1404661416)| <a name="com.swedbankpay.mobilesdk.merchantbackend/MerchantBackendProblem.Server/instance/#/PointingToDeclaration/"></a> [androidJvm] val [instance](index.md#1295215756%2FProperties%2F-1404661416): [String](https://kotlinlang.org/api/latest/jvm/stdlib/kotlin/-string/index.html)?RFC 7807 default property: a URI reference that identifies the specific occurrence of the problem   <br>|
| <a name="com.swedbankpay.mobilesdk.merchantbackend/MerchantBackendProblem.Server/jsonObject/#/PointingToDeclaration/"></a>[jsonObject](index.md#-152576486%2FProperties%2F-1404661416)| <a name="com.swedbankpay.mobilesdk.merchantbackend/MerchantBackendProblem.Server/jsonObject/#/PointingToDeclaration/"></a> [androidJvm] val [jsonObject](index.md#-152576486%2FProperties%2F-1404661416): JsonObjectThe raw RFC 7807 object parsed as a Gson JsonObject.   <br>|
| <a name="com.swedbankpay.mobilesdk.merchantbackend/MerchantBackendProblem.Server/raw/#/PointingToDeclaration/"></a>[raw](index.md#638460497%2FProperties%2F-1404661416)| <a name="com.swedbankpay.mobilesdk.merchantbackend/MerchantBackendProblem.Server/raw/#/PointingToDeclaration/"></a> [androidJvm] val [raw](index.md#638460497%2FProperties%2F-1404661416): [String](https://kotlinlang.org/api/latest/jvm/stdlib/kotlin/-string/index.html)The raw RFC 7807 object.   <br>|
| <a name="com.swedbankpay.mobilesdk.merchantbackend/MerchantBackendProblem.Server/status/#/PointingToDeclaration/"></a>[status](index.md#-1649679153%2FProperties%2F-1404661416)| <a name="com.swedbankpay.mobilesdk.merchantbackend/MerchantBackendProblem.Server/status/#/PointingToDeclaration/"></a> [androidJvm] val [status](index.md#-1649679153%2FProperties%2F-1404661416): [Int](https://kotlinlang.org/api/latest/jvm/stdlib/kotlin/-int/index.html)?RFC 7807 default property: the HTTP status codeThis should always be the same as the actual HTTP status code reported by the server.   <br>|
| <a name="com.swedbankpay.mobilesdk.merchantbackend/MerchantBackendProblem.Server/title/#/PointingToDeclaration/"></a>[title](index.md#1421807393%2FProperties%2F-1404661416)| <a name="com.swedbankpay.mobilesdk.merchantbackend/MerchantBackendProblem.Server/title/#/PointingToDeclaration/"></a> [androidJvm] val [title](index.md#1421807393%2FProperties%2F-1404661416): [String](https://kotlinlang.org/api/latest/jvm/stdlib/kotlin/-string/index.html)?RFC 7807 default property: a short summary of the problem.   <br>|
| <a name="com.swedbankpay.mobilesdk.merchantbackend/MerchantBackendProblem.Server/type/#/PointingToDeclaration/"></a>[type](index.md#875546503%2FProperties%2F-1404661416)| <a name="com.swedbankpay.mobilesdk.merchantbackend/MerchantBackendProblem.Server/type/#/PointingToDeclaration/"></a> [androidJvm] val [type](index.md#875546503%2FProperties%2F-1404661416): [String](https://kotlinlang.org/api/latest/jvm/stdlib/kotlin/-string/index.html)RFC 7807 default property: a URI reference that identifies the problem type.   <br>|


## Inheritors  
  
|  Name | 
|---|
| <a name="com.swedbankpay.mobilesdk.merchantbackend/MerchantBackendProblem.Server.MobileSDK///PointingToDeclaration/"></a>[MerchantBackendProblem.Server](-mobile-s-d-k/index)|
| <a name="com.swedbankpay.mobilesdk.merchantbackend/MerchantBackendProblem.Server.SwedbankPay///PointingToDeclaration/"></a>[MerchantBackendProblem.Server](-swedbank-pay/index)|
| <a name="com.swedbankpay.mobilesdk.merchantbackend/MerchantBackendProblem.Server.Unknown///PointingToDeclaration/"></a>[MerchantBackendProblem.Server](-unknown/index)|
