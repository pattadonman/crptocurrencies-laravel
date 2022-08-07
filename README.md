# crptocurrencies-laravel
crptocurrencies-laravel-backend-db

1.install xampp 

2.install composer

3.install vscode

4.install php

5.นำfolder crpto-laravel ไปใส่ใน htdocs

6.แก้ไข connection database ใน .env

7.run command line ใน terminal ด้วย php artisan migrate เพือ สร้าง database

8.run command line  ใน terminal ด้วย ตามลำดับบรรทัดที่ละบรรทัด
php artisan db:seed --class=IdCardsSeeder
php artisan db:seed --class=AddressCardsSeeder
php artisan db:seed --class=IdCardsSeeder
php artisan db:seed --class=UserLoginSeeder
php artisan db:seed --class=TradeStoresSeeder
php artisan db:seed --class=PersonalInformationsSeeder
php artisan db:seed --class=OrderTradeOperationsSeeder

เพื่อseed ข้อมูลเพื่อทดสอบ

9.เปิดbrowser เติมurl ดังนี้เพื่อเช็ดความสัมพันธ์ของdatabase ex. one to one ,one to many ที่ละบรรทัด
http://localhost:8000/show_one_to_many_idUser_to_tradeStore
http://localhost:8000/show_one_to_many_userLogin_to_idCard
http://localhost:8000/show_one_to_many_userLogin_to_OrderTradeOperation
http://localhost:8000/show_one_to_one_PersonalInformation_to_idUser_table
http://localhost:8000/show_one_to_one_idCard_to_addressCard_table
http://localhost:8000/show_one_to_one_user_to_idCard_table
