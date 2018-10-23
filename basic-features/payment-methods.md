# Payment Methods

{% hint style="info" %}
You must create a payment method before you can open your shop.
{% endhint %}

## Setting up a payment method

1\) Go to the payment methods page.

Click **Enterprises** in the blue horizontal menu, and then click **Manage** next to your enterprise. Then, click **Payment methods** in the menu on the left hand side.

2\) Click on the **create new payment method** button.

3\) Tick your enterprise, in the box on the right hand side of the page titled Hubs. This indicates which enterprise the payment method you are about to create will apply to. You can select more than one enterprise.

4\) **Name:** Choose a name for this payment method. \(i.e. Pay with credit card using Paypal, Cash on delivery or Bank Transfer etc\). It will be displayed at checkout and on customers' order confirmation emails.

5\) **Description:** provide further details about the payment method. For example, for a bank transfer, you would provide details of the bank account. This description will be displayed at checkout and in order confirmation emails.

The screenshot below shows a payment methods display at checkout. The customer has selected ‘cash on collection/delivery’ and the ‘correct change…’ description is displayed.

![](https://openfoodnetwork.org/wp-content/uploads/2015/05/Payment-at-checkout.png)

6\) **Active:** Select whether this payment method is currently visible and available, or not.

7\) **Tags:** Use tag rules if you want to make certain payment methods available/unavailable for specific customers \(e.g. wholesale vs retail\). See [tags and tag rules](../advanced-features/shop-setup/tags-and-tag-rules.md) for more information.

8\) **Payment providers**: Select the one which is relevant to the payment method you are creating.

You can accept payment via 5 payment options:

* Cash/EFT/etc. \(Use this for payments which occur after checkout, externally to OFN such as cash or bank transfers\)
* MasterCard Internet Gateway Service \(MIGS\)
* PayPal Express
* [Pin Payments](https://pin.net.au/)
* Stripe

If you have selected ‘Cash/EFT/etc..’ as the provider, click **Create** to end the process.

### Payment Providers

For MasterCard, Paypal and Pin Payments additional instructions are below.

{% tabs %}
{% tab title="Paypal" %}
To setup a PayPal payment method, you need a PayPal business or merchant account. You can create one [here](https://www.paypal.com/au/webapps/mpp/merchant). Once you have that, you can set up ‘API access’ within PayPal, which will enable OFN to connect customers directly with your PayPal account.

1. Login to your PayPal Account
2. Click Tools and then select API credentials

![](https://openfoodnetwork.org/wp-content/uploads/2015/05/Paypal-tools-API-credentials.png)

1. Click on ‘View API Signature’  and you will see the API details you’ll need to set up Paypal in OFN.

![](https://openfoodnetwork.org/wp-content/uploads/2015/05/API-Access.png)

![](https://openfoodnetwork.org/wp-content/uploads/2015/05/Api-Signature.png)

1. In OFN, make sure you are logged in as your Enterprise User. Go to an Enterprise and create a Payment Method. Select PayPal and fill in the details from the PayPal site.

**Login:**Type the API Username.

**Password:**Type the API Password.

**Signature:**Type the Signature in this field.

![](https://openfoodnetwork.org/wp-content/uploads/2015/05/New-Payment-Paypal-1.png)

**Server:** Change the ‘server’ field to ‘live’ – this is case sensitive.

**Solution:** Solution determines whether or not a user needs a PayPal account to check out.

Type “Mark” if you do want users to have a paypal account, or “Sole” if they can checkout without a Paypal account \(with credit card\).

**Landing Page:** You can select which page to show customers once they’re redirected to PayPal.

Type “Login” to direct customer to the login form for PayPal \(if you selected “Mark” above\). Or type “Billing” to show show customers a form where they can enter their credit card data and possibly sign up for a PayPal account \(if you selected “Sole” above\).
{% endtab %}

{% tab title="MIGS" %}
 MasterCard Internet Gateway Service \(MIGS\)

Set up of this service needs to be done through your bank. So far it has been tested with Bendigo Bank.
{% endtab %}

{% tab title="Stripe" %}
[Stripe](https://stripe.com/au) is an online payment platform similar to Paypal. It will allow you to accept credit card payments from your customers. Stripe is a global platform, but is only available on certain OFN instances. Contact your [local OFN team](https://openfoodnetwork.org/ofn-local/) to see whether it’s available on your OFN.

#### Why use Stripe?

Stripe is simple to setup for shop owners and is reasonably priced. The fees charged by Stripe vary in each country; [Australia](https://stripe.com/au/pricing), [Canada](https://stripe.com/ca/pricing), [France](https://stripe.com/fr/pricing), [UK](https://stripe.com/gb/pricing), [USA](https://stripe.com/us/pricing).

Stripe is also easy for customers to use. Unlike Paypal, when the customer checks out, they don’t need to login with Paypal to place their order, rather they just need to enter their card details and then complete their order.

Stripe is the recommended payment method for shops who wish to use [**subscriptions** ](../advanced-features/subscriptions/)on OFN, as Stripe allows customers to give permission to a shop to automatically bill their credit card for subscription orders. This isn’t offered by Paypal, Pin or MIGS payment platforms.

#### Setup

**Connect with Stripe**

Before you can setup a payment method that uses Stripe, you’ll need to Connect with Stripe. To do this, click on the ‘Connect with Stripe’ button.

![](https://openfoodnetwork.org/wp-content/uploads/2017/08/Connect-with-Stripe.png)

You’ll be taken to a form to fill in your details. If you already have an account with Stripe, you can login, if not, fill in the form to create a Stripe account.

The information you’ll be asked for includes: country, a description of your business, your Business address and ABN, your personal details and your bank account \(where received payments will be deposited\).

**Create a New Payment Method**

Once you’ve connected with Stripe, you can then create a payment method which will work with your connected account.

Treat the **Name**, **Description**, **Active** and **Tags** fields as you would with any payment method.

**Provider:** Select Stripe.

Once you select Stripe, ‘Provider Settings’ will be shown.

**Stripe Account Owner:**

Select the enterprise that has a Stripe account connected.

If you select an enterprise that is not Connected to Stripe \(see above\) , you will get the error shown below. Either click ‘Connect One’ or return to your Payment Methods tab to Connect with Stripe. See instructions above.

![](https://openfoodnetwork.org/wp-content/uploads/2017/08/Stripe-connect.png)

#### Stripe Payments for Customers

When customers checkout in a shop and pay with a Stripe payment method, they’ll have the options of selecting a tickbox allowing their credit card details to be stored against their account \(if they are logged in\).

Customer can also save a credit card in their Account, or delete saved ones.

![](https://openfoodnetwork.org/wp-content/uploads/2017/08/Add-card.png)

When the customer next shops with an OFN shop offering Stripe as a payment method, they’ll be able to select from their saved credit cards.

**Viewing and redeeming your payments via Stripe**

When a customer pays for their order with Stripe, the funds \(minus Stripe's fees\) will go to your stripe account. Depending on your setting in Stripe the funds will be automatically transferred to your chosen bank account periodically.

**Taking further payment**

If you need to take additional payment from a customer because they have further balance due,  you can create an invoice in Stripe. The customer will get sent an email asking for them to pay with Credit/Debit card. This won't be communicated to OFN, so you'll need to mark the payment off manually.

![](../.gitbook/assets/image%20%2822%29.png)
{% endtab %}

{% tab title="Pin Payments" %}
For Pin Payments you only require your API key. You need to set up an account with Pin Payments first, and can get a discount by signing up as an OFN member \([https://pin.net.au/partners/open-food-network/signup](https://pin.net.au/partners/open-food-network/signup)\)

**API Key:**Enter your “Live Secret API Key’ here – you can find this in your PinPayments account \(see below\). First from your account, select API Keys. Then once you have generated an API key, copy the ‘Live Secret API Key’ and paste it into the API key field in OFN.

![API Keys](https://openfoodnetwork.org/wp-content/uploads/2015/05/API-Keys.png)

![API Key](https://openfoodnetwork.org/wp-content/uploads/2015/05/API-2.png)

**Server:**Type ‘live’ – this is case sensitive.
{% endtab %}
{% endtabs %}

### Fees on Payment Methods

![Calculator](https://openfoodnetwork.org/wp-content/uploads/2015/05/Calculator.png)

You can attach a fee to payment methods. Most commonly this is used to pass on a platform's fees to the customer, such as Paypal fees.  
1. Select a fee calculator \(full descriptions below\)  
2. Enter the value.

_Note: Payment method fees do not include tax._

#### Fee Calculators

**Flat Percent:**  This fee is charged as a percentage of the total amount charged in the order.

**Flat Rate \(per order\):** This fee is applied as standard fee to all orders, regardless of the size of the order.

**Flexible Rate** – This calculator is typically used for promotional discounts where you charge a reduced fee as the customer makes more purchases.

* ‘First Item Cost’: The fee charged for the first item in the order.
* ‘Additional Item Cost’: The fee charged for items beyond the first item.
* ‘Max Items’: The maximum number of items on which the fee will be applied. Items purchased beyond this amount will be not be charged the fee.

For example: If the first cost is $2, Additional Item Cost is $1 and the maximum items is three. If a customer orders 5 items, they will be charged $2 for the first item, $1 for the second and third, and no fee for the fourth and fifth.

**Flat Rate \(per item\):** This fee is a constant fee, applied to products listed as ‘items’. \(it will not be applied to products listed as per kg, or per L\)

**Price Sack:** This fee is used to charge a discount on fees for orders which exceed a certain dollar amount.

* ‘Minimum Amount’: If the order’s total is below this amount, they will be charged the ‘Normal Amount’.
* ‘Discount Amount’: Orders which are equal to or greater than the minimum amount will be charged the ‘Discount Amount’.

