# Introduction-3

The goal of this documentation is to describe the services, systems and strategies used by basico.com with Shopify its eCommerce Platform.

By default, Shopify does not provide clear ways to setup a Brazilian eCommerce with efficience and clarity.

After hours studying the possibilities provided by Shopify in terms of API, Webhooks and Integrations, we decided to create 3 sub-applications to support our eCommerce Lifesystem.

They are:

* Basico Shipping App
* Basico NF App
* Basico Payment App

## I will explain more about them in the following lines.

## 1 - Basico Shipping App

Today at basico.com, we use what Shopify understand as "CarrierCalculated Rates", which is basically a dynamic way to calculate the Order Shipping based on which products you have on your shopping cart.

Shopify today offers 2 static ways of calculating shipping options: by "Weight Range", and by "Order Total Range".

Also, you can Setup a Fixed Shipping amount, but its not our case.

### So, what this app Does?

This App allow us to have Full control about which rules we will enable in our Shipping Service. This solution Nullify the Shipping management section at Shopify Admin, since we cannot configure our Shipping Rules by Shopify Admin anymore, but it give us full flexibility to decide which rules we want to apply on our customer checkout.

This way we can create customized rules for Free Freight, Fixed Rates \(Loggi\), or even prices coming directly from Correios.

Solving the Shipping problem, we move to the next section...

---

## 2 - Basico NF App \(Brazilian Invoices\)

Today at basico.com, we use a B2B service known as "Bling", which allow us to generate the Brazilian Invoice and emit it directly on the Brazilian Government systems. We decided to use this B2B service, because we understand that there are a lot of bureaucracies required to make this work.

At Shopify, there are no native tools to help us on this \(except for a TinyERP App\), and furthermore, we didnt wanted to change all of our Invoice Generation Flow just because we are moving from one Platform to another.

### So, what this app Does?

This App allow us to have Full control about which tool we will use to control and generate our Customer Invoices.

Solving the Invoice problem, we move to the next section...

---

## 3 - Basico Payment App \(Brazilian Payments\)

Today at basico.com, we use a Payment Gateway called Adyen, which is supported by a local merchant called Cielo. Unfortunately, Shopify does not allow us to use Adyen seamlessly. As Brazilian merchants we feel that Shopify was forcing us to change our Payment Gateway negociation just because they have a poor brazilian support. We dont want that, thats why we are going to create this app.

### So, what this app Does?

This app allow us to have Full control about which Gateway we want to use on our payment. It allow us to support Payment Partners which are not supported by Shopify natively. Shopify argues that its very difficult to mantain support to several Gateways, so they do it Slowly, and always though ActiveMerchant.

With this app, we can choose which Merchant we will support, and do it through a transparent checkout, as we have today.

