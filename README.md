# Introduction

The goal of this documentation is to describe the services, systems and strategies used by basico.com with Shopify its eCommerce Platform.

By default, Shopify does not provide clear ways to setup a Brazilian eCommerce with efficience and clarity.

After hours studying the possibilities provided by Shopify in terms of API, Webhooks and Integrations, we decided to create 3 sub-applications to support our eCommerce Lifesystem.

---

## 1 - Basico Shipping App

Today at basico.com, we use what Shopify understand as "CarrierCalculated Rates", which is basically a dynamic way to calculate the Order Shipping based on which products you have on your shopping cart.

Shopify today offers 2 static ways of calculating shipping options: by "Weight Range", and by "Order Total Range".

Also, you can Setup a Fixed Shipping amount, but its not our case.

### So, what this app Does?

This App allow us to have Full control about which rules we will enable in our Shipping Service. This solution Nullify the Shipping management section at Shopify Admin, since we cannot configure our Shipping Rules by Shopify Admin anymore, but it give us full flexibility to decide which rules we want to apply on our customer checkout.

This way we can create customized rules for Free Freight, Fixed Rates \(Loggi\), or even prices coming directly from Correios.

Solving the Shipping problem, we move to the next section...

---

## 1 - Basico NF App \(Brazilian Invoices\)

Today at basico.com, we use a B2B service known as "Bling", which allow us to generate the Brazilian Invoice and emit it directly on the Brazilian Government systems. We decided to use this B2B service, because we understand that there are a lot of bureaucracies required to make this work here,

