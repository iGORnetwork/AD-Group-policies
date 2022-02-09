# AD-Group-policies
## DC1
1)Запретите анимацию при первом входе пользователей в систему на всех клиентских компьютерах домена.
а)Создаем групповую политику Tools → group policy management → Moscow.wsr → create a gpo in this domain, and link it here → Add Name Animation. 
![](https://github.com/iGORnetwork/AD-Group-policies/blob/main/DC1-1.png)
б)Отключен анимацию в политике Tools → group policy management → Moscow.wsr → Animation → Edit → policies → administrative templates → system → logon → show first sign-in animation → disabled.
![](https://github.com/iGORnetwork/AD-Group-policies/blob/main/DC1-2.png)
c)Применение групповой политики Tools → group policy management → Moscow.wsr → IT → link an existing gpo → Animation → ok
![](https://github.com/iGORnetwork/AD-Group-policies/blob/main/DC1-3.png)
2)Члены группы IT должны быть членами группы локальных администраторов на всех клиентских компьютерах домена.             
а)Создаем групповую политику Tools → group policy management → Moscow.wsr → create a gpo in this domain, and link it here → Add Name IT
![](https://github.com/iGORnetwork/AD-Group-policies/blob/main/DC1-4.png)
б)Настраиваем политику Tools → group policy management → Moscow.wsr → IT → Edit → policies → windows settings → security settings → restricted groups → add groups → Name IT → ok
![](https://github.com/iGORnetwork/AD-Group-policies/blob/main/DC1-5.png)
с)Применяем политику к группе this group is a member → add → Browse → administrator → ок → aply → ok 
![](https://github.com/iGORnetwork/AD-Group-policies/blob/main/DC1-6.png)
d)Проверяем CLI1 Saha
![](https://github.com/iGORnetwork/AD-Group-policies/blob/main/CLI1-1.png)
3) в браузерах Microsoft Edge должна быть настроена стартовая страница – www.moskow.wsr
a) Создаем групповую политику Tools → group policy management → Moscow.wsr → create a gpo in this domain, and link it here → name homePage → ок
![](https://github.com/iGORnetwork/AD-Group-policies/blob/main/DC1-7.png)
b) Настраиваем политику Tools → group policy management → Moscow.wsr → homePage → Edit → policies → administrative → templates windows → components microsoft → edge configure home page → enabled → www.moskow.wsr → apply → ok
![](https://github.com/iGORnetwork/AD-Group-policies/blob/main/DC1-8.png)
c) Применяем политику Tools → group policy management → Moscow.wsr → homePage → Edit → user configuration → preferences → control panel → settings internet settings → new → internet explorer 10 → www.moskow.wsr → Start homePage → apply → ok 
![](https://github.com/iGORnetwork/AD-Group-policies/blob/main/DC1-9.png)
d) Проверяем CLI1 Saha
![](https://github.com/iGORnetwork/AD-Group-policies/blob/main/CLI1-10.png)
4) все пользователи при первом входе в домен с компьютера CLI1 должны видеть на рабочем столе ярлык программы Калькулятор.
а)Создаем групповую политику Tools → group policy management → Moscow.wsr → create a gpo in this domain, and link it here → Add Name Calculator → ok

б)Настраиваем политику Tools → group policy management → Moscow.wsr → IT → Edit → policies → windows settings → Shortcuts → New Shortcut 
![](https://github.com/iGORnetwork/AD-Group-policies/blob/main/DC1-12.png)
c) Применяем политику 
![](https://github.com/iGORnetwork/AD-Group-policies/blob/main/DC1-13.png)
d)Проверяем CLI1 Saha
