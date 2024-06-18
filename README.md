# data-domain-design-checkout

Domain Desgin for online store

need to implement shopping cart - overview

1. create cart

Add products to storage and save until checkout. Storage can be online session, anonymous db storage, logged in db storage

Shopping cart pulls in items selected.  If logged in account, gets user info.

Allow incrment/decrement/remove for items in cart

Check inventory if required.

2. create/link to user

If not logged in, create account/login

3. create order

Get address for shipping and sales tax - new or guest, add address, existing, offer ability to update.

Sales tax differs by location, i.e. California requires sales tax to be collected from California residents based on County of residence (for most online sales).  There are APIs tbat can be used to find sales tax.

If shipping is required calculate that now. If there are shipping options, show them now.

4. payment - PCI DSS compliance

Get save payment info for logged in users

Collect payment info for Guest/new user. Allow logged in users to update payment info.

What payment options are there? Credit card? Paypal? Venmo? Zelle? Bitcoin?

5. accept order

Final acceptance of order triggers payment, pick ticket (if applicable), shipping labels, tracking number, thank you and tracking email sent, inventory/production system integration.


I have created a lucidchart UML document.  I am at the point where I would share what I have so far and ask if changes are needed, so I guess that is what I am doing with you.
