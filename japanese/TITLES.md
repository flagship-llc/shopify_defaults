# メール件名（title）一覧＜日本語版（国内向け）＞

#### 補足事項
* 国内向けに変更した箇所はCountryの除去のみです。


## Order（注文関係のお客様向けメール） 

1. Order confirmation 
{{name}} ご注文完了

2. Order canceled 
{{ name }} ご注文がキャンセルされました

3. Order refund 
返金処理手続き完了のお知らせ

4. Draft order invoice 
{{ name }} ご注文内容

5. Abandoned checkout 
購入手続きを完了する

6. Gift card created 
{{ shop.name }}のギフトカード


## Shipping（配送関係のお客様向けメール） 

7. Fulfillment request（未翻訳） 
Order fulfillment request for {{ shop_name }} 

8. Shipping confirmation 
{{ name }} 配送のお知らせ

9. Shipping Update 
{{ name }} 配送のお知らせ

10. Shipment out for delivery（未翻訳）
A shipment from order {{ name }} is out for delivery 

11. Shipment delivered（未翻訳）
A shipment from order {{ name }} has been delivered 


## Customer（ユーザーアカウント関係のお客様向けメール） 

12. Customer account invite 
アカウント登録のご連絡

13. Customer account welcome 
お客様情報の確認

14. Customer account password reset 
パスワード再登録のご連絡

15. Contact customer 
{{ shop.name }}からお客様へ


## Order Notifications（運営者向け通知メール） 

16. New order（未翻訳）
[{{shop_name}}] Order {{ name }} placed by {{ billing_address.name }}{% if has_high_risks? %} (Risk of fraud){% endif %} 

17. New order (mobile)（未翻訳）
Order {{ name }} 
