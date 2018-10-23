# Order Cycles \(for Hubs\)

_\*Not a Hub, but a producer? See_ [_Order Cycles for producers_](order-cycles-for-producers.md)_._

You open you shop by creating an Order Cycle. When you make an order cycle you select when you shop is open \(from and until\), which products will go into the shop, and any fees that you'll apply.

**Why Order Cycles?**  
Some hubs may wish to have an online store which is perpetually open, and to fulfill orders on a one by one basis, as they are received. However, many hubs operate on a periodic ordering system, which allows them to process orders in bulk, making their packing and distribution activities more efficient. Let’s use an example to illustrate a common periodic ordering cycle structure.

**Order Cycle Example**

For instance, each Monday morning a hub might assess the availability of their stock for the week. Based on this information they will create an order cycle by Monday afternoon and open their store. Customers can then place orders in their store, until the order cycle closes on Wednesday at midnight. On Thursday all of the orders can be packed by the hub and prepared for delivery on Friday. The following week the cycle will begin again, and with the creation of a new order cycle. By structuring order cycles in this way, and dealing with orders in bulk, hubs can make their ordering, sorting, packing and transport activities much more efficient than if they process orders individually as they are placed.

## Access Order Cycles

You can create an order cycle, and view previous order cycles by clicking on **Manage Order Cycles** on your dashboard.

![](https://openfoodnetwork.org/wp-content/uploads/2015/05/Order-Cycle.png)

Or from the horizontal menu at the top of the page.

![Access order cycle](https://openfoodnetwork.org/wp-content/uploads/2015/05/Access-order-cycle.png)

## Create a New Order Cycle

Below is the first stage in creating an order cycle.

\*Remember, you cannot create an order cycle until you have set up [shipment](shipping-methods.md) and [payment](https://github.com/ofn-user-guide/ofn-user-guide-master/tree/d5a1113e673b0e22198ca207b1db61339799868a/payment-methods-2.md) methods.

![Set order cycle coordinator](https://openfoodnetwork.org/wp-content/uploads/2015/05/Set-coordinator.png)

Select the coordinator of the order cycle. The enterprise which coordinates an order cycle has full powers and permissions to edit and manage an order cycle. Other enterprises involved in the order cycle \(such as suppliers or distributors\) have restricted abilities to edit an order cycle \(for more information click here\). After the coordinator is selected, the subsequent order cycle will be restricted according to who has granted this coordinator permission to add them to an order cycle \(P-OC\).For more information about Enterprise to Enterprise permissions go here.

**Name \(**_**required**_**\):**Give your order cycle a name which is meaningful to you. We recommend that you follow a consistent naming protocol e.g FoodHub\_Week27\_2014. We also recommend that you include the name of your hub in the order cycle name, so that OFN support can identify your order cycles if you need assistance.

**Orders Open:** This is the date at when your OFN store will be open, visible and start to accept orders from customers.

**Order Close:** This is the date when your OFN store will close and stop accepting orders. If you intend to have an order cycle which is continuously open, select a close date which is well into the future.

**Add Coordinator Fee:**As a hub, the coordinator is most likely you. Here you can apply your Enterprise Fee which acts as the markup. The fee will be calculated according to the calculator selected in [Enterprise Fees](enterprise-fees.md). You can only apply an enterprise fee which has previously been created.

![New order cycle fields](https://openfoodnetwork.org/wp-content/uploads/2015/05/New-order-cycle-3.png)

### Incoming: select producer and produce

The incoming section is where you can select the producers, and their produce, which will be available in this order cycle. In the dropdown menu you will see all producers who have granted you permission to add their produce to your order cycle \(See _Relationships with Producers_ section for details\). After selecting a supplier and clicking **Add Supplier** all of the products associated with that supplier will be visible. Check those products you wish to add to the store, or click **select all.** Note: Products which have an ‘on hand’ value of zero \(no stock available\) will still be visible, so be careful to check that you have adequate on hand inventory for the products selected.

![Incoming](https://openfoodnetwork.org/wp-content/uploads/2015/05/Incomiing.png)

The **Receival Details** fields are optional. If you wish to use the **Notify Produers** button, to send orders to your supplying producers, you should write your stock receival instructions here. \(more info in the Notify Producers section at the bottom of this page\).

The **Add Fee** button is where you can apply an enterprise fee, belonging to that supplier. Select the name of the enterprise in the first dropdown box, then click the name of the enterprise fee in the second dropdown box. In the example below, an enterprise fee named OrderAdmin is applied to the Producer of Fruit.

This fee will be applied to all of the Producer of Fruit’s products which are purchased. The fee is calculated according to the fee calculator which was selected when the [Enterprise Fee](enterprise-fees.md) was created.

![Apply enterprise fee to incoming supplier](https://openfoodnetwork.org/wp-content/uploads/2015/05/Enterprise-Fee.png)

### Outgoing: select distributor

The distributor\(s\) selected in the outgoing section, will have a shopfront opened from this order cycle. In simple hub models, there is only one distributor, the hub. So select the hub in the distributor column, and then select all products that should be visible in the online store during this order cycle. More complex hubs might have buying groups, in which case each is selected as a distributor, and will consequently have their own shopfront created. You then have the capacity to select specific products to be available in each buying group’s shop.

![Outgoing Section](https://openfoodnetwork.org/wp-content/uploads/2015/05/Outoging-New.png)

The **tags** column is where you can tag your order cycles to customise whether they are visible/invisible to certain customers. See [tags and tag rules](https://github.com/coopdevs/guia-usuaris-katuma/tree/44e128f05a3e2f656a055ff5a68d3d8cfe7c2229/advanced-features/shop-setup/tags-and-tag-rules.md) for more information.

The **‘ready for \(ie Date/Time\)’ \(**_**required**_**\):** This box tells the customer when their order will be ready for either collection or delivery. If your order cycle is a perpetual one, which fulfills orders on an individual basis rather then in bulk, you should enter something like ‘Two days after order is received’. The example below shows how ‘Friday 9th’ is displayed in a store.

![ready for field](https://openfoodnetwork.org/wp-content/uploads/2015/05/Ready-for.png)

The note is also shown at check out, when the customer selects their shipping method \(see below\) and is included in the order confirmation email.

![Ready for info in email](https://openfoodnetwork.org/wp-content/uploads/2015/05/shipping-info.png)

The **Pick-Up Instructions** message will be included in the customer’s order confirmation email, below the message that corresponds to their chosen shipping method \(see below\). This note is designed to only be visible to customers, so you can include more sensetive information like addresses, or phone numbers etc. See below for an example of the order confirmation email.

![collection details message](https://openfoodnetwork.org/wp-content/uploads/2015/05/Collection-details.png)

**Add Fee:** Again, a previously created enterprise fee can be assigned to this distributor.

### Open the shopfront

Click Create to save this order cycle.

> Note: When you create an order cycle, and the opening and closing dates fall either side of the present, a shopfront will become live on the homepage. If you are not ready to have your store open, temporarily put the opening and closing dates in the past \(this can be edited when you are ready to open\).

For periodic, repetitive order cycles, you can copy an existing order cycle and change the dates, to make the process quicker. See below.

![duplicate an order cycle](https://openfoodnetwork.org/wp-content/uploads/2015/05/copy-order-cycle.png)

> Note: It might be tempting to use the same OC all the time, and simply update the dates each time you reopen it. However, it's better to create a new Order Cycle, or duplicate and update an OC each time you have a new OC. If you always use the same OC, you will find that you can't filter your reports by OC. This can limit how effectively you can use OFN reports.

Order cycles will display as green when they are active, yellow when schedules for a future date, and grey when they have closed. When an order cycle close over one month ago, it will no longer display on this list. To view all of your past order cycles click ‘show more’ at the top of the list.

**‘Notify Producers’ Button**

Some hubs use this tool as a way to notify their suppliers of which items have been ordered, in what quantities and also to give them receival instructions. Clicking this button will send the following email to the contact email of the producer’s profile. It is sent to all producers included in this order cycle and will sum all of the orders placed in that order cycle.

_Dear**&lt;Producer’s Name&gt;**,_

_We now have all the consumer orders for next food drop._

_Stock pickup/delivery instructions: **&lt;Receival instructions&gt;**._

## Orders summary

_Here is a summary of the orders for your products:_

_**&lt;Total products orders in this order cycle \(example below\)&gt;**  
– Producer of Meat – Leg of Lamb \(Frozen\) \(1.5kg\) \(QTY: 1\) @ $22.50 = $22.50  
– Producer of Meat – Sausages \(100g\) \(QTY: 3\) @ $3.00 = $9.00_

_Thanks and best wishes,_

_**&lt;Hub Name, address, phone number, email&gt;**_

## Advanced Features

Related advanced features:

* The [inventory ](https://github.com/coopdevs/guia-usuaris-katuma/tree/44e128f05a3e2f656a055ff5a68d3d8cfe7c2229/advanced-features/products/inventory-tool.md)tool allows a shop to 'override' the inherent price and stock level of a product. You can use this tool if you want to track stock levels seperately across two shops, or have different prices for the same product in different shops.
* [Creating ‘display only’ order cycles](https://github.com/coopdevs/guia-usuaris-katuma/tree/44e128f05a3e2f656a055ff5a68d3d8cfe7c2229/advanced-features/order-cycles/display-only-order-cycles.md)
* [Permissions in multi-enterprise order cycles](https://github.com/coopdevs/guia-usuaris-katuma/tree/44e128f05a3e2f656a055ff5a68d3d8cfe7c2229/advanced-features/collaboration-with-other-enterprises/permissions-in-multi-enterprise-order-cycles.md)

