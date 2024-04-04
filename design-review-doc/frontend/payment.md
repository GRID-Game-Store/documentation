## Table of Contents

* [Task Overview](#task-overview)
* [Code Review Process](#code-review)
* [Shame File](#shame-file)

## Task Overview <a name="task-overview"></a>
* Payment with the help of Stripe, PayPal, and balance in site and recharge balance.
* Payment with the help of Stripe, PayPal, and Balance.
* Revert transaction when the client cancels payment.


## Code Documentation <a name="code-review"></a>
* Cart page
* Modal checkout (when you click on "Buy All")
* Select Payment method (Radio buttons, because you can select only one method, the default value is a Stripe)
* Payment with help payment system plus balance, doesn't work with payment method "balance"
* Get the balance on the account to disable the checkbox payment with the payment system plus the balance
* Button wich to send in server `POST` on `/checkout` 
* When we receive data from `POST` checkout we redirect to the payment system page and if the balance payment method is you redirect to the success page
* When you pay on the page Stripe or PayPal you are redirected to the success page or failed page
* Success page to send `POST` on `/capture` with sessionId in params
* Failed page to send `POST` on `/cancelTransaction` with sessionId in params
## Shame File  <a name="shame-file"></a>
![image](https://github.com/GRID-Game-Store/documentation/assets/60855065/d95d53dd-8b1f-44ae-b196-46f3180a38c6)




