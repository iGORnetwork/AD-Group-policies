# AD-Group-policies
## GPO
1) Запретите анимацию при первом входе пользователей в систему на всех клиентских компьютерах домена
а) Создаем групповую политику Tools → group policy management → Moscow.wsr → create a gpo in this domain, and link it here → Add Name Animation. 
![](https://github.com/iGORnetwork/AD-Group-policies/blob/main/DC1-1.png)
б) Отключен анимацию в политике Tools → group policy management → Moscow.wsr → Animation → Edit → policies → administrative templates → system → logon → show first sign-in animation → disabled.
![](https://github.com/iGORnetwork/AD-Group-policies/blob/main/DC1-2.png)
c) Применение групповой политики Tools → group policy management → Moscow.wsr → IT → link an existing gpo → Animation → ok
![](https://github.com/iGORnetwork/AD-Group-policies/blob/main/DC1-3.png)
