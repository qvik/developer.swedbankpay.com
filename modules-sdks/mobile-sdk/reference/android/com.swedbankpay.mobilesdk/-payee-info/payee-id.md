---
title: payeeId -
---
//[sdk](../../../index)/[com.swedbankpay.mobilesdk](../index)/[PayeeInfo](index)/[payeeId](payee-id)



# payeeId  
[androidJvm]  
Content  
@SerializedName(value = payeeId)  
  
val [payeeId](payee-id): [String](https://kotlinlang.org/api/latest/jvm/stdlib/kotlin/-string/index.html)  
More info  


The unique identifier of this payee set by Swedbank Pay.



This is usually the Merchant ID. However, usually best idea to set this value in your backend instead. Thus, this property defaults to the empty string, but it is included in the data model for completeness.

  


