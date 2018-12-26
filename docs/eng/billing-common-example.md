Ruslan - the owner of the gym in which there are two rooms - a strength gym and fitness.
Ruslan becomes a client of Billingolang. From the point of view of the Billingolang system, Ruslan is our User.

Of course that Ruslan may have several gyms, and even in different cities (divisions), and in each of them there are employees who will interact with Billingolang on a specific system, and access rights. But obout this not in this section.

1. Ruslan fills in his and / or his company data including possible forms of payments, storing keys for selected payment extensions (addons). Suppose that the credit cards are accepted through Stripe Gateway.
2. Ruslan forms two products - Strength gym and Fitness.
3. Ruslan associates previously activated payment methods with each product:
* for Strength gym - Stripe & Braintree & PayPal & Wire transfer & Bitcoin & DASH & Monero. 
* for Fitness - Stripe & Braintree & PayPal & Wire transfer
4. Ruslan creates the following plans and connects them with the product Strength gym :
  - One-time training Strength gym:
    - Type: One-time
    - Price - 3 euro
    - Frequency of payment - one-time payment
  - Weekly training Strength gym:
    - Type: Recurring
    - Price - 10 euro
    - Frequency of payment - once a week
  - Crescent training Strength gym:
    - Type: Recurring
    - Price - 15 euro
    - Frequency of payment - once in half a month
  - Monthly training Strength gym:
    - Type: Recurring
    - Price 25 euro
    - Frequency of payment - once a month
5. Ruslan creates the following plans and associates them with the Fitness product:

  5.1. Yoga:

  * One-time training Yoga:
    * Type: One-time
    * Price - 4 euro
    * Frequency of payment - one-time payment
  * Weekly training Yoga:
    * Type: Recurring 
    * Price - 12 euro
    * Frequency of payment - once a week
  * Crescent training Yoga:
    * Type: Recurring
    * Price - 17 euro
    * Frequency of payment - once in half a month
  * Monthly training Yoga:
    * Type: Recurring
    * Price 27 euro
    * Frequency of payment - once a month

  5.2. Pilates:

  * One-time training Pilates:
    * Type: One-time
    * Price - 5 euro
    * Frequency of payment - one-time payment
  * Weekly training Pilates:
    * Type: Recurring
    * Price - 13 евр
    * Frequency of payment - once a week
  * Crescent training Pilates:
    * Type: Recurring
    * Price - 18 euro
    * Frequency of payment - once in half a month
  * Monthly training Pilates:
    * Type: Recurring
    * Price 28 euro
    * Frequency of payment - once a month

6. Ruslan forms the following extensions and connects them with products:

   | Расширения                    | Описание                                 | Продукты              |
   | :---------------------------- | -----------------------------------------| --------------------- |
   | Personal Trainer Strength gym | Price - 10 euro per hour                 | Strength gym          |
   | Personal Trainer Yoga         | Price - 12 euro per hour                 | Fitness               |
   | Personal Trainer Pilates      | Price - 13 euro per hour                 | Fitness               |
   | Towel                         | Price - 0.5 euro                         | Strength gym, Fitness |
   | Foot Massage                  | Duration 15 minutes<br />Price -15 euro  | Strength gym, Fitness |
   | Back Massage                  | Duration 15 minutes<br />Price -15 euro  | Strength gym, Fitness |
   | Full Massage                  | Duration 30 minutes<br />Price - 30 euro | Strength gym, Fitness |

7. Kirill is a client of Ruslan. From the point of view of Billingolang - Ruslans customer.

8. Kirill on Ruslan’s own website, or on Ruslan’s website integrated into our system, chooses three one-time subscriptions to the Strength gym product for himself and two repeated Yoga subscriptions for his wife and Pilates for his daughter, with some extensions, simply marking them:

   - [x] One-time training Strength gym
     - [x] Type One-time subscription
     - [x] Quantity 3
     - [x] Price - 3 euro
     - [x] Frequency of payment - one-time payment
   - [x] Monthly training Yoga
     - [x] Type: Recurring
     - [x] Quantity 1
     - [x] Price 27 euro
     - [x] Frequency of payment - once a month
   - [x] Monthly training Pilates
     - [x] Type: Recurring
     - [x] Quantity 1
     - [x] Price 28 euro
     - [x] Frequency of payment - once a month
   - [x] Personal Trainer Yoga
     - [x] Quantity 4 часа
     - [x] Price - 12 euro per hour
     - [x] Frequency of payment - once a month
   - [x] Full Massage
     - [x] Quantity 4
     - [x] Price - 30 euro
     - [x] Frequency of payment - once a month

9. Kirill chooses one or several available payment methods previously identified by Ruslan.

10. Billingolang forms invoices for payment and sends them to Ruslan and Kirill. If necessary, integrating them into the accounting system of Ruslan.

11. Billingolang consistently conducts Kirill through the first payment for each subscription.

12. Billingolang starts repeating (recurring) billing for recurring subscriptions on the saved data of payment add-ons entered by Kirill during first payment.