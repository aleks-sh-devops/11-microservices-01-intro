# Домашнее задание к занятию "Введение в микросервисы"

## Задача 1: Интернет Магазин

Руководство крупного интернет магазина у которого постоянно растёт пользовательская база и количество заказов рассматривает возможность переделки своей внутренней ИТ системы на основе микросервисов. 

Вас пригласили в качестве консультанта для оценки целесообразности перехода на микросервисную архитектуру. 

Опишите какие выгоды может получить компания от перехода на микросервисную архитектуру и какие проблемы необходимо будет решить в первую очередь.

## Ответ  
Преимущества:  
- Возможность использовать разные технологии + тестировать разные технологии + переходить на разные технологии  
- Повышение отказоустойчивости системы за счет разбиения одного монолита на несколько независимых микросервисов + изолирование этих сервисов друг от друга  
- Возможность маштабирования конкретных нагруженных участков, а не всей системы, в целом  
- Более гибкая возможность распределения нагрузки, в том числе, за счет балансировщиков  
- возможность частого обновления софта + возможность обновления не всей системы, а лишь отдельных микросервисов не влияя на всю систему, что приводит к более честым релизам  
- Возможность разбиения спецов на команды, которые будут отвечать за конкретный сервис (в дальнейшем это приведет к более глубокому знанию не тратя время на посторонние задачи)  
- Упрощение интеграции с другими системами  
- Возможность организации оркестрации и хореографии  

Возможные подводные камни:  
- Разворачивание системы мониторинга и сбора логов, бэкапов по серверам и сервисам  
- Необходимо продумать отказоустойчивую инфраструктуру  
- Обучение сотрудников, поскольку для микросервисов требуются соответствующий квалифицированный персонал (возможно, нужно заранее разбить сотрудников для команд в микросервисы)  
- Определиться каким образом будем делить наше монолитное приложение на микросервисы  
- Какие протоколы интеграции будут использоваться, какие подходы к безопасности необходимо применить, а также взаимодействие (синхронное или асинхронное) и оркестрация или хореография  
- Разворачивание системы для хранения базы знаний о том или ином микросервисе дабы избежать фактора автобуса
