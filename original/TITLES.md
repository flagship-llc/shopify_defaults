# メール件名（title）一覧

## Order

1. Order confirmation 
Order {{name}} confirmed 

2. Order canceled 
Order {{ name }} has been canceled 

3. Order refund 
Refund notification 

4. Draft order invoice 
Invoice {{name}} 

5. Abandoned checkout 
Complete your Purchase 

6. Gift card created 
Your {{ shop.name }} gift card is ready! 


## Shipping 

7. Fulfillment request 
Order fulfillment request for {{ shop_name }} 

8. Shipping confirmation 
A shipment from order {{ name }} is on the way 

9. Shipping Update 
Shipping update for order {{ name }} 

10. Shipment out for delivery 
A shipment from order {{ name }} is out for delivery 

11. Shipment delivered 
A shipment from order {{ name }} has been delivered 


## Customer 

12. Customer account invite 
Customer account activation 

13. Customer account welcome 
Customer account confirmation 

14. Customer account password reset 
Customer account password reset 

15. Contact customer 
Message from {{ shop.name }} 


## Order Notifications 

16. New order 
[{{shop_name}}] Order {{ name }} placed by {{ billing_address.name }}{% if has_high_risks? %} (Risk of fraud){% endif %} 

17. New order (mobile) 
Order {{ name }} 
