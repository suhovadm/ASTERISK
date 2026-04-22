Типовые схемы (оператор / enterprise-уровень).  

Варик 1 (самый частый, SBC + Kamailio + FreeSWITCH / Asterisk):  

Внешний мир (операторы / SIP trunk).  
        │  
        ▼  
SBC (например, Oracle SBC или AudioCodes).  
        │  
        ▼  
Kamailio (SIP routing / core).  
        │  
        ▼  
FreeSWITCH / Asterisk (логика звонка, IVR, конференции).  
        │  
        ▼  
Пользователи / приложения.  

Роли:  
Oracle SBC.  
Oracle Communications Session Border Controller.  
•	Стоит на границе сети.  
•	Первый контакт с внешним миром.  
•	Безопасность, NAT, транскодинг, защита.  
Kamailio.  
•	Внутренний SIP routing core.  
•	Маршрутизация, балансер, регистрация.  
•	«Мозг» сигнализации.  
FreeSWITCH.  
•	Обрабатывает сам звонок.  
•	IVR, конференции, запись, логика.  

Более реалистичные варианты.  
Варик 2 (упрощённый).  
SIP trunk / Внешний мир – Kamailio – FreeSWITCH / Asterisk – Пользователи / приложения.  

Варик 3 (ещё более упрощённый).  
SIP trunk / Внешний мир – SBC – FreeSWITCH / Asterisk – Пользователи / приложения.  
