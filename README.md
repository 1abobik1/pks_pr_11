# Практическая работа № 11 (программирование корпоративных систем)

выполнил: **Берлов Дмитрий Максимович**

группа: **ЭФБО-02-22**

## Описание и этапы выполнения работы

В данной работе необходимо было подключить Supabase и использовать для авторизации пользователя в магазине.

1) Добавил supabase в зависимости проекта, используя команду ```flutter pub add supabase_flutter```
2) Создал аккаунт в supabase
3) В **main.dart** создал подключение

```
void main() async{
  await Supabase.initialize(
      url: 'https://pxebqdevfyhznspqkvmp.supabase.co',
      anonKey: 'eyJhbGciOiJIUzI1NiIsInR5cCI6IkpXVCJ9.eyJpc3MiOiJzdXBhYmFzZSIsInJlZiI6InB4ZWJxZGV2Znloem5zcHFrdm1wIiwicm9sZSI6ImFub24iLCJpYXQiOjE3MzEzOTQzMDksImV4cCI6MjA0Njk3MDMwOX0.H_3nRXcVbsVnKJDv7wAnFto_dDxN-hLQwaJyC4mnFhc'
  );
  runApp(const MyApp());
}
```

4) Сверстал дополнительные страницы: страницу профиля (если пользователь не вошел в систему), страницу входа, страницу регистрации
5) Если пользователь не авторизован он все равно может просматривать страницу каталога

<img src='https://github.com/user-attachments/assets/74138c0b-3edb-4e17-b3fd-e93b23ab4a45' width = 300 />

<img src='https://github.com/user-attachments/assets/368dccc4-cfaa-45e2-8fa2-2f2606fb467d' width = 300 />

6) После нажатия на кнопку "Войти в аккаунт" пользователь попадет на страницу входа

<img src='https://github.com/user-attachments/assets/27790fe4-dac7-43d5-8d5c-3a6385babaf4' width = 300 />

<img src='https://github.com/user-attachments/assets/14ca2eb1-922e-4756-b14c-92be8d23e372' width = 300 />

7) Если пользователь уже зарегистрирован, то его данные отобразятся в профиле

<img src='https://github.com/user-attachments/assets/540e5dac-6e0a-404d-bc27-abd6c8cdba86' width = 300 />

8) Если у пользователя нет аккаунта, то необходимо зарегистрироваться

<img src='https://github.com/user-attachments/assets/b0941e88-f8ad-498d-982c-dafc29311cd9' width = 300 />

<img src='https://github.com/user-attachments/assets/a5e8af90-46e6-409c-8fb1-431d71416084' width = 300 />

9) После регистрации пользователь сможет зайти в свой аккаунт

<img src='https://github.com/user-attachments/assets/08143dba-3d74-41ad-9883-05e2efc50361' width = 300 />
