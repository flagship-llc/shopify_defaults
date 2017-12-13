# Email title list (English and Japanese)


## Order（注文関係のお客様向けメール） 

1. Order confirmation 
{% assign curLang = attributes.LS_language %}{% if curLang == 'en' %}Order {{name}} confirmed{% elsif curLang == 'ja' %}{{name}} ご注文完了{% else %}Order {{name}} confirmed{% endif %}

2. Order canceled 
{% assign curLang = attributes.LS_language %}{% if curLang == 'en' %}Order {{ name }} has been canceled{% elsif curLang == 'ja' %}{{ name }} ご注文がキャンセルされました{% else %}Order {{ name }} has been canceled{% endif %}

3. Order refund 
{% assign curLang = attributes.LS_language %}{% if curLang == 'en' %}Refund notification{% elsif curLang == 'ja' %}返金処理手続き完了のお知らせ{% else %}Refund notification{% endif %}

4. Draft order invoice 
{% assign curLanguage = customer.tags | join: '' | split: 'ls~' %}{% assign curLang = curLanguage[1] %}{% if curLang == 'en' %}Invoice {{name}}{% elsif curLang == 'ja' %}{{ name }} ご注文内容{% else %}Invoice {{name}}{% endif %}

5. Abandoned checkout 
{% assign curLang = attributes.LS_language %}{% if curLang == 'en' %}Complete your Purchase{% elsif curLang == 'ja' %}購入手続きを完了する{% else %}Complete your Purchase{% endif %}

6. Gift card created 
{% assign curLanguage = gift_card.customer.tags | join: '' | split: 'ls~' %}{% assign curLang = curLanguage[1] %}{% if curLang == 'en' %}Your {{ shop.name }} gift card is ready!{% elsif curLang == 'ja' %}{{ shop.name }}のギフトカード{% else %}Your {{ shop.name }} gift card is ready!{% endif %}

* No Japanese translation for [POS and mobile receipt]. 


## Shipping（配送関係のお客様向けメール） 

7. Fulfillment request (No Japanese translation) 
Order fulfillment request for {{ shop_name }} 

8. Shipping confirmation 
{% assign curLang = attributes.LS_language %}{% if curLang == 'en' %}A shipment from order {{ name }} is on the way{% elsif curLang == 'ja' %}{{ name }} 配送のお知らせ{% else %}A shipment from order {{ name }} is on the way{% endif %}

9. Shipping Update 
{% assign curLang = attributes.LS_language %}{% if curLang == 'en' %}Shipping update for order {{ name }}{% elsif curLang == 'ja' %}{{ name }} 配送のお知らせ{% else %}Shipping update for order {{ name }}{% endif %}

10. Shipment out for delivery (No Japanese translation)
A shipment from order {{ name }} is out for delivery 

11. Shipment delivered (No Japanese translation)
A shipment from order {{ name }} has been delivered 


## Customer（ユーザーアカウント関係のお客様向けメール） 

12. Customer account invite 
{% assign curLanguage = customer.tags | join: '' | split: 'ls~' %}{% assign curLang = curLanguage[1] %}{% if curLang == 'en' %}Customer account activation{% elsif curLang == 'ja' %}アカウント登録のご連絡{% else %}Customer account activation{% endif %}

13. Customer account welcome 
{% assign curLanguage = customer.tags | join: '' | split: 'ls~' %}{% assign curLang = curLanguage[1] %}{% if curLang == 'en' %}Customer account confirmation{% elsif curLang == 'ja' %}お客様情報の確認{% else %}Customer account confirmation{% endif %}

14. Customer account password reset 
{% assign curLanguage = customer.tags | join: '' | split: 'ls~' %}{% assign curLang = curLanguage[1] %}{% if curLang == 'en' %}Customer account password reset{% elsif curLang == 'ja' %}パスワード再登録のご連絡{% else %}Customer account password reset{% endif %}

15. Contact customer 
{% assign curLanguage = customer.tags | join: '' | split: 'ls~' %}{% assign curLang = curLanguage[1] %}{% if curLang == 'en' %}Message from {{ shop.name }}{% elsif curLang == 'ja' %}{{ shop.name }}からお客様へ{% else %}Message from {{ shop.name }}{% endif %}


## Order Notifications（運営者向け通知メール） 

16. New order(No Japanese translation)
[{{shop_name}}] Order {{ name }} placed by {{ billing_address.name }}{% if has_high_risks? %} (Risk of fraud){% endif %} 

17. New order (mobile)(No Japanese translation)
Order {{ name }} 
