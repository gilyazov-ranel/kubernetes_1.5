### Задание 1. Создать Deployment приложений backend и frontend

1. Создать Deployment приложения _frontend_ из образа nginx с количеством реплик 3 шт.
2. Создать Deployment приложения _backend_ из образа multitool. 
<img width="1066" height="132" alt="image" src="https://github.com/user-attachments/assets/0064661d-1f2b-4932-b75c-e251672764a8" />

3. Добавить Service, которые обеспечат доступ к обоим приложениям внутри кластера. 
4. Продемонстрировать, что приложения видят друг друга с помощью Service.
<img width="1351" height="638" alt="image" src="https://github.com/user-attachments/assets/9a84c611-9875-4481-853b-707586f696f9" />

5. Предоставить манифесты Deployment и Service в решении, а также скриншоты или вывод команды п.4.

------

### Задание 2. Создать Ingress и обеспечить доступ к приложениям снаружи кластера

1. Включить Ingress-controller в MicroK8S.
2. Создать Ingress, обеспечивающий доступ снаружи по IP-адресу кластера MicroK8S так, чтобы при запросе только по адресу открывался _frontend_ а при добавлении /api - _backend_.
3. Продемонстрировать доступ с помощью браузера или `curl` с локального компьютера.
4. Предоставить манифесты и скриншоты или вывод команды п.2.
<img width="1429" height="319" alt="image" src="https://github.com/user-attachments/assets/7027b67f-84d8-4475-962a-f6d0b60ee6a0" />
<img width="1406" height="584" alt="image" src="https://github.com/user-attachments/assets/bc2d7101-6e5a-4151-a083-f81896085eb3" />

при попытке разных обращений к curl при помощи nodePorta получаю ошибку 
<img width="916" height="178" alt="image" src="https://github.com/user-attachments/assets/eefee556-7185-4f49-b85c-a2cd7f5ace00" />
<img width="1149" height="175" alt="image" src="https://github.com/user-attachments/assets/d53fe912-7e27-474a-bf2b-6896f08aef3e" />
