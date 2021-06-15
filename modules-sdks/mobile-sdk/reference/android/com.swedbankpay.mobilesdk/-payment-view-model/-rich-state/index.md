---
title: RichState -
---
//[sdk](../../../../index)/[com.swedbankpay.mobilesdk](../../index)/[PaymentViewModel](../index)/[RichState](index)



# RichState  
 [androidJvm] class [RichState](index)

Contains the state of the payment process and possible associated data.

   


## Properties  
  
|  Name |  Summary | 
|---|---|
| <a name="com.swedbankpay.mobilesdk/PaymentViewModel.RichState/exception/#/PointingToDeclaration/"></a>[exception](exception)| <a name="com.swedbankpay.mobilesdk/PaymentViewModel.RichState/exception/#/PointingToDeclaration/"></a> [androidJvm] val [exception](exception): [Exception](https://kotlinlang.org/api/latest/jvm/stdlib/kotlin/-exception/index.html)?If the current state is [RETRYABLE_ERROR](../-state/-r-e-t-r-y-a-b-l-e_-e-r-r-o-r/index), or [FAILURE](../-state/-f-a-i-l-u-r-e/index) caused by an [Exception](https://kotlinlang.org/api/latest/jvm/stdlib/kotlin/-exception/index.html), this property contains that exception.   <br>|
| <a name="com.swedbankpay.mobilesdk/PaymentViewModel.RichState/failingUri/#/PointingToDeclaration/"></a>[failingUri](failing-uri)| <a name="com.swedbankpay.mobilesdk/PaymentViewModel.RichState/failingUri/#/PointingToDeclaration/"></a> [androidJvm] val [failingUri](failing-uri): [Uri](https://developer.android.com/reference/kotlin/android/net/Uri.html)?If the current state is [FAILURE](../-state/-f-a-i-l-u-r-e/index), and it was caused by a failing redirect, this property contains the redirect [Uri](https://developer.android.com/reference/kotlin/android/net/Uri.html) that failed to load.   <br>|
| <a name="com.swedbankpay.mobilesdk/PaymentViewModel.RichState/redirectErrorCode/#/PointingToDeclaration/"></a>[redirectErrorCode](redirect-error-code)| <a name="com.swedbankpay.mobilesdk/PaymentViewModel.RichState/redirectErrorCode/#/PointingToDeclaration/"></a> [androidJvm] val [redirectErrorCode](redirect-error-code): [Int](https://kotlinlang.org/api/latest/jvm/stdlib/kotlin/-int/index.html)?If the current state is [FAILURE](../-state/-f-a-i-l-u-r-e/index), and it was caused by a failing redirect, the error code describing the failure.   <br>|
| <a name="com.swedbankpay.mobilesdk/PaymentViewModel.RichState/redirectErrorDescription/#/PointingToDeclaration/"></a>[redirectErrorDescription](redirect-error-description)| <a name="com.swedbankpay.mobilesdk/PaymentViewModel.RichState/redirectErrorDescription/#/PointingToDeclaration/"></a> [androidJvm] val [redirectErrorDescription](redirect-error-description): [String](https://kotlinlang.org/api/latest/jvm/stdlib/kotlin/-string/index.html)?If the current state is [FAILURE](../-state/-f-a-i-l-u-r-e/index), and it was caused by a failing redirect, a textual description of the failure.   <br>|
| <a name="com.swedbankpay.mobilesdk/PaymentViewModel.RichState/redirectHttpErrorReason/#/PointingToDeclaration/"></a>[redirectHttpErrorReason](redirect-http-error-reason)| <a name="com.swedbankpay.mobilesdk/PaymentViewModel.RichState/redirectHttpErrorReason/#/PointingToDeclaration/"></a> [androidJvm] val [redirectHttpErrorReason](redirect-http-error-reason): [String](https://kotlinlang.org/api/latest/jvm/stdlib/kotlin/-string/index.html)?If the current state is [FAILURE](../-state/-f-a-i-l-u-r-e/index), and it was caused by an error http response to a redirect, the reason phrase of that respone.   <br>|
| <a name="com.swedbankpay.mobilesdk/PaymentViewModel.RichState/redirectHttpErrorStatus/#/PointingToDeclaration/"></a>[redirectHttpErrorStatus](redirect-http-error-status)| <a name="com.swedbankpay.mobilesdk/PaymentViewModel.RichState/redirectHttpErrorStatus/#/PointingToDeclaration/"></a> [androidJvm] val [redirectHttpErrorStatus](redirect-http-error-status): [Int](https://kotlinlang.org/api/latest/jvm/stdlib/kotlin/-int/index.html)?If the current state is [FAILURE](../-state/-f-a-i-l-u-r-e/index), and it was caused by an error http response to a redirect, the status code of that response.   <br>|
| <a name="com.swedbankpay.mobilesdk/PaymentViewModel.RichState/retryableErrorMessage/#/PointingToDeclaration/"></a>[retryableErrorMessage](retryable-error-message)| <a name="com.swedbankpay.mobilesdk/PaymentViewModel.RichState/retryableErrorMessage/#/PointingToDeclaration/"></a> [androidJvm] val [retryableErrorMessage](retryable-error-message): [String](https://kotlinlang.org/api/latest/jvm/stdlib/kotlin/-string/index.html)?If the current state is [RETRYABLE_ERROR](../-state/-r-e-t-r-y-a-b-l-e_-e-r-r-o-r/index), this property contains an error message describing the situation.   <br>|
| <a name="com.swedbankpay.mobilesdk/PaymentViewModel.RichState/state/#/PointingToDeclaration/"></a>[state](state)| <a name="com.swedbankpay.mobilesdk/PaymentViewModel.RichState/state/#/PointingToDeclaration/"></a> [androidJvm] val [state](state): [PaymentViewModel.State](../-state/index)The state of the payment process.   <br>|
| <a name="com.swedbankpay.mobilesdk/PaymentViewModel.RichState/terminalFailure/#/PointingToDeclaration/"></a>[terminalFailure](terminal-failure)| <a name="com.swedbankpay.mobilesdk/PaymentViewModel.RichState/terminalFailure/#/PointingToDeclaration/"></a> [androidJvm] val [terminalFailure](terminal-failure): [TerminalFailure](../../-terminal-failure/index)?If the current state is [FAILURE](../-state/-f-a-i-l-u-r-e/index), and it was caused by an onError callback from the Chekout API, this property contains an object describing the error.   <br>|
| <a name="com.swedbankpay.mobilesdk/PaymentViewModel.RichState/updateException/#/PointingToDeclaration/"></a>[updateException](update-exception)| <a name="com.swedbankpay.mobilesdk/PaymentViewModel.RichState/updateException/#/PointingToDeclaration/"></a> [androidJvm] val [updateException](update-exception): [Exception](https://kotlinlang.org/api/latest/jvm/stdlib/kotlin/-exception/index.html)?If the current state is [IN_PROGRESS](../-state/-i-n_-p-r-o-g-r-e-s-s/index), and an attempt to update the payment order failed, the cause of the failure.   <br>|
| <a name="com.swedbankpay.mobilesdk/PaymentViewModel.RichState/viewPaymentOrderInfo/#/PointingToDeclaration/"></a>[viewPaymentOrderInfo](view-payment-order-info)| <a name="com.swedbankpay.mobilesdk/PaymentViewModel.RichState/viewPaymentOrderInfo/#/PointingToDeclaration/"></a> [androidJvm] val [viewPaymentOrderInfo](view-payment-order-info): [ViewPaymentOrderInfo](../../-view-payment-order-info/index)?If the current state is [IN_PROGRESS](../-state/-i-n_-p-r-o-g-r-e-s-s/index) or [UPDATING_PAYMENT_ORDER](../-state/-u-p-d-a-t-i-n-g_-p-a-y-m-e-n-t_-o-r-d-e-r/index), the [ViewPaymentOrderInfo](../../-view-payment-order-info/index) object describing the current payment order.   <br>|
