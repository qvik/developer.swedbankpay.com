{% assign operation_title = include.operation_title %}
{% assign documentation_section = include.documentation_section  %}

{%- assign operation_title_field_name = operation_title | capitalize -%}

{% if operation_title != "create-payment" %}

{:.code-header}
**{{ operation_title_field_name }}**

{:.table .table-striped}
| XLSX                            | XML                     | API                                                                             |
| :------------------------------ | :---------------------- | :------------------------------------------------------------------------------ |
| `Swedbank Pay Batch Number`     | `SwedbankbatchNo`       |                                                                                 |
| `Transaction Number`            | `TransactionNo`         | `transaction.number`                                                            |
| `Order id`                      | `OrderId`               | `transaction.payeeReference`                                                    |
| `Date Created`                  | `DateCreated`           | `transaction.created`                                                           |
| `Date Modified`                 | `DateModified`          |{% if documentation_section=="swish" or documentation_section=="invoice" %}`transaction.created`{% endif %}                                                                                                                                      |
| `Provider`                      | `Provider`              |                                                                                 |
| `Type`                          | `Type`                  |                                                                                 |
| `Amount`                        | `Amount`                | `transaction.amount`                                                            |
| `Currency`                      | `Currency`              |{% if operation_title == "create-payment" %}`payment.currency`{% endif %}        |
| `Product Number`                | `MerchantProductNo`     |                                                                                 |
| `Description`                   | `Description`           |{% unless documentation_section=="mobile-pay" %} `transaction.description` {% endunless %}                                                                                                                                            |
| `VAT Amount`                    | `VATAmount`             |{% unless operation_title == "sale" %} `transaction.vatAmount` {% endunless %}                                                                                                                                            |
| `VAT Percentage`                | `VatoPercentage`        |                                                                                 |
| `Credit Card Batch Number`      | `CreditCardBatchNo`     |                                                                                 |
| `Direct Debit Bank Reference`   | `DirectDebitbankRef`    |{% if documentation_section=="card" or documentation_section=="payment-menu" or documentation_section=="checkout" %}`transaction.number` if DirectDebit {% endif%}                                                            |
| `Reference`                     | `Reference`             |{% if documentation_section=="card" or documentation_section=="payment-menu" or documentation_section=="checkout" %}`transaction.number` if DirectDebit {%endif%}                                                             |
| `Swedbank Account Number`       | `SwedbankAccountNo`     |                                                                                 |
| `Referenced Transaction Number` | `ReferencedTransaction` |{% unless operation_title=="reversal" %}`transaction.number` if reversed later{% endunless %}                                                                                                                                            |
| `Sales Channel`                 | `SalesChannel`          |                                                                                 |
| `Brand`                         |                         |                                                                                 |
| `Point Of Sale`                 |                         |                                                                                 |

{% endif %}

{% if operation_title == "create-payment" %}

{:.code-header}
**Create Payment**

{:.table .table-striped}
| XLSX                            | XML                     | API                                                                             |
| :------------------------------ | :---------------------- | :------------------------------------------------------------------------------ |
| `Swedbank Pay Batch Number`     | `SwedbankbatchNo`       |                                                                                 |
| `Transaction Number`            | `TransactionNo`         |                                                                                 |
| `Order id`                      | `OrderId`               | {% if documentation_section =="swish" %} `payeeInfo.payeeReference` {% endif %} |
| `Date Created`                  | `DateCreated`           |                                                                                 |
| `Date Modified`                 | `DateModified`          |                                                                                 |
| `Provider`                      | `Provider`              |                                                                                 |
| `Type`                          | `Type`                  |                                                                                 |
| `Amount`                        | `Amount`                |                                                                                 |
| `Currency`                      | `Currency`              | `payment.currency`                                                              |
| `Product Number`                | `MerchantProductNo`     |                                                                                 |
| `Description`                   | `Description`           |                                                                                 |
| `VAT Amount`                    | `VATAmount`             |                                                                                 |
| `VAT Percentage`                | `VatoPercentage`        |                                                                                 |
| `Credit Card Batch Number`      | `CreditCardBatchNo`     |                                                                                 |
| `Direct Debit Bank Reference`   | `DirectDebitbankRef`    |                                                                                 |
| `Reference`                     | `Reference`             |                                                                                 |
| `Swedbank Account Number`       | `SwedbankAccountNo`     |                                                                                 |
| `Referenced Transaction Number` | `ReferencedTransaction` |                                                                                 |
| `Sales Channel`                 | `SalesChannel`          |                                                                                 |
| `Brand`                         |                         |                                                                                 |
| `Point Of Sale`                 |                         |                                                                                 |

{% endif %}