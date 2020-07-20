# Shopping Basket Discount Task

## What is the Task?
The coding exercise is the second stage of our technical interview process. We want it to be as real world as possible so research and use the resources necessary. 

Feel free to take as long as you feel you need to on this task, we understand that not everyone has a huge amount of time while others feel they want to spend longer to demonstrate everything they can. 

Note your decisions, constraints and thoughts in a readme to help us understand your process.

## Why do we ask for the Task?

The coding exercise allows us to view your work in the most realistic way we can, giving you a chance to show us your problem solving skills. There are many approaches to the task. Being able to talk over the approach, options and considerations in the final stage of our interview helps us understand your thought process.

## Requirements
The company issues two types of voucher for customers to gain discounts on shopping baskets. 

Gift Voucher:
- Can be redeemed against the value of a basket. 
- Multiple gift vouchers can be applied to a basket.
- Gift vouchers can only be redeemed against non gift voucher products.
- The purchase of a gift voucher does not contribute to the discountable basket total.

Offer vouchers:
- Requires a threshold that needs to be exceeded before a discount can be applied e.g. £5.00 off of baskets over £50.
- Only a single offer voucher can be applied to a basket.
- Can be applicable to only a subset of products.

Offer and Gift vouchers can be used in conjunction. If a customer applies an offer voucher to a basket that will not satisfy the threshold or a customer removes item/changes an items quantity resulting in a voucher not being valid then a message will need to be displayed to the customer.

Write an application that represents a basket and has the ability to handle the following scenarios:

---

### Basket 1:

1 Jumper @ £54.65

1 Head Light (Head Gear Category of Product)  @ £3.50

**Sub Total: £58.15**

No vouchers applied

**Total: £58.15**

---

### Basket 2:

1 Gloves @ £10.50

1 Jumper @ £54.65

**Sub Total: £65.15**

1 x £5.00 Gift Voucher XXX-XXX applied

**Total: £60.15**

---

### Basket 3:

1 Gloves @ £25.00

1 Jumper @ £26.00

**Sub Total: £51.00**

1 x £5.00 off Head Gear in baskets over £50.00 Offer Voucher YYY-YYY applied

**Total: £51.00**

**Message:** “There are no products in your basket applicable to Offer Voucher YYY-YYY.”

---

### Basket 4:

1 Gloves @ £25.00

1 Jumper @ £26.00

1 Head Light (Head Gear Category of Product)  @ £3.50

**Sub Total: £54.50**

1 x £5.00 off Head Gear in baskets over £50.00 Offer Voucher YYY-YYY applied

**Total: £51.00**

---

### Basket 5:

1 Gloves @ £25.00

1 Jumper @ £26.00

**Sub Total: £51.00**

1 x £5.00 Gift Voucher XXX-XXX applied

1 x £5.00 off baskets over £50.00 Offer Voucher YYY-YYY applied

**Total: £41.00**

---

### Basket 6:

1 Gloves @ £25.00

1 £30 Gift Voucher @ £30.00

**Sub Total: £55.00**

1 x £5.00 off baskets over £50.00 Offer Voucher YYY-YYY applied

**Total: £55.00**

**Message:** “You have not reached the spend threshold for Gift Voucher YYY-YYY. Spend another £25.01 to receive £5.00 discount from your basket total.”

---

### Basket 7:

1 Gloves @ £25.00

**Sub Total: £25.00**

1 x £30.00 Gift Voucher XXX-XXX applied

**Total: £0.00**

---

## Deliverables
You are required to build code that represents a basket along with a set of tests. This can be a console app, a class library or Rest API. You should not create a mobile app, website or UI for this application. There is no need to create a database for this application.

Feel free to take as long as you feel you need to on this task, we understand that not everyone has a huge amount of time while others feel they want to spend longer to demonstrate everything they can.  We do however ask the task is ideally returned within 7 days of being sent.

When submitting the task please also provide an estimate of how long you feel you spent on the work so we can put the work into context.

You can submit the test in the following ways:
- From a shared link such as drop box, one drive, google drive etc. (preferred)
- Shared via a public git repository

**When sharing via email or a shared link** please zip up your solution with the following name format: [YourNameHere] - BasketTest
