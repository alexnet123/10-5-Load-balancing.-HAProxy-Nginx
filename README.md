# Домашнее задание к занятию "`10-5-Load-balancing.-HAProxy-Nginx`" - `Вахрамеев А.В.`

---

### Задание 1.

Что такое балансировка нагрузки и зачем она нужна? 

*Приведите ответ в свободной форме.*

---

### Задание 2.

Чем отличаются между собой алгоритмы балансировки round robin и weighted round robin? В каких случаях каждый из них лучше применять? 

*Приведите ответ в свободной форме.*

---

### Задание 3.

Установите и запустите haproxy.

*Приведите скриншот systemctl status haproxy, где будет видно, что haproxy запущен.*

---

### Задание 4.

Установите и запустите nginx.

*Приведите скриншот systemctl status nginx, где будет видно, что nginx запущен.*

---

### Задание 5.

Настройте nginx на виртуальной машине таким образом, чтобы при запросе:

`curl http://localhost:8088/ping`

он возвращал в ответе строчку: 

"nginx is configured correctly"

*Приведите скриншот получившейся конфигурации.*

---

## Дополнительные задания (со звездочкой*)

Эти задания дополнительные (не обязательные к выполнению) и никак не повлияют на получение вами зачета по этому домашнему заданию. Вы можете их выполнить, если хотите глубже и/или шире разобраться в материале.

---

### Задание 6*.

Настройте haproxy таким образом, чтобы при ответе на запрос:

`curl http://localhost:8080/`

он проксировал его в nginx на порту 8088, который был настроен в задании 5 и возвращал от него ответ: 

"nginx is configured correctly". 

*Приведите скриншот получившейся конфигурации.*
