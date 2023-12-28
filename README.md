# TOIB-3

# Отчет по практической работе №3

# Rsyslog. Сервер

1 На виртуальных машинах настроил сеть на Сетевой мост
2 На первой виртуальной машине скачем rsyslog


![Desktop Screenshot 2023 11 09 - 15 05 24 04](https://github.com/hipster-x/TOIB-3/assets/145153023/111e690f-1d04-4a33-a9f8-2d3855dc7379)


3 Запустим сервис. Проверим работоспособность 

 ![Desktop Screenshot 2023 11 09 - 15 06 24 90](https://github.com/hipster-x/TOIB-3/assets/145153023/27dd620b-a172-44b6-a462-830cf5dcde9c)

4 Настраиваем rsyslog для удаленного приема системного журнала

![Desktop Screenshot 2023 11 09 - 15 37 31 43](https://github.com/hipster-x/TOIB-3/assets/145153023/5a8bf58e-73ea-4e7c-b953-18dbae96a5ec)

5 Перезапускаем сервис

![Desktop Screenshot 2023 11 09 - 16 02 57 25](https://github.com/hipster-x/TOIB-3/assets/145153023/b71d91d6-9487-4113-aa2f-d7576e1af4fe)


# Rsyslog. Клиент

1 На второй виртуальной машине скачаем rsyslog

![Desktop Screenshot 2023 11 09 - 16 11 17 67](https://github.com/hipster-x/TOIB-3/assets/145153023/c4636599-8621-4519-a9a9-40d5f8570a89)

2 Отредактируем config, добавляем правило для пересылки логов

![Desktop Screenshot 2023 11 09 - 16 16 26 35](https://github.com/hipster-x/TOIB-3/assets/145153023/ed6b3c6a-1b29-463e-afb5-2a153086a90c)

3 Перезапускаем сервис

![Desktop Screenshot 2023 11 09 - 16 18 45 22](https://github.com/hipster-x/TOIB-3/assets/145153023/e9e52dc6-2dc5-43a8-85f7-89e576f3bf9d)

# Loki

1 Разворачиваем на сервере Loki

![Desktop Screenshot 2023 11 09 - 16 42 53 54](https://github.com/hipster-x/TOIB-3/assets/145153023/fb798f90-fd68-4581-aa3a-4e14a81b9a1c)

2 На клиенте устанавлиеваем Promtail

![Desktop Screenshot 2023 11 09 - 17 15 13 38](https://github.com/hipster-x/TOIB-3/assets/145153023/44c92d3b-1497-477d-9b9d-cd2aebf7feb1)

3 Создаем файл конфинфигурации 

![Desktop Screenshot 2023 11 09 - 17 19 07 05](https://github.com/hipster-x/TOIB-3/assets/145153023/888a8d82-ce7a-4603-bf30-eea0a47259cd)

4 Создаем Unit

![Desktop Screenshot 2023 11 09 - 17 19 58 45](https://github.com/hipster-x/TOIB-3/assets/145153023/f35076e2-7606-497f-983c-4142a3b5f0f9)

![Desktop Screenshot 2023 11 09 - 17 44 19 47](https://github.com/hipster-x/TOIB-3/assets/145153023/18f6bc66-8104-40c5-b93e-daf76a41481d)

5 Перезапускаем сервис

![Desktop Screenshot 2023 11 09 - 17 46 30 49](https://github.com/hipster-x/TOIB-3/assets/145153023/282b24b3-2582-4018-9cec-ed80ec98717b)

6 Посмотрим логи на сервере

![Desktop Screenshot 2023 11 09 - 17 53 00 08](https://github.com/hipster-x/TOIB-3/assets/145153023/6809aa3d-7dbb-4dfc-9045-65fc948f515f)

![Desktop Screenshot 2023 11 09 - 17 51 42 19](https://github.com/hipster-x/TOIB-3/assets/145153023/09ec86bd-901a-44e4-bad9-41981d5d9227)

# Signoz

1 Запускаем контейнер на сервере 

![Desktop Screenshot 2023 11 09 - 18 04 05 44](https://github.com/hipster-x/TOIB-3/assets/145153023/945812f1-8e2a-4d69-ba1f-a717b9e10f3f)

![Desktop Screenshot 2023 11 09 - 18 07 38 58](https://github.com/hipster-x/TOIB-3/assets/145153023/c0ea6d34-212b-4760-948d-02ee2e40b8a8)

2 Так же для клиента (редактируем docker-compose файл)

![Desktop Screenshot 2023 11 09 - 18 37 35 23](https://github.com/hipster-x/TOIB-3/assets/145153023/ef1a953b-678b-4ff4-9918-16a633061c09)

3 Запускаем контейнер

![Desktop Screenshot 2023 11 09 - 18 40 53 44](https://github.com/hipster-x/TOIB-3/assets/145153023/59cf0f3c-6869-4da4-b576-322595d66839)

4 Наблюдаем логи в SigNoz

![Desktop Screenshot 2023 11 09 - 18 42 44 17](https://github.com/hipster-x/TOIB-3/assets/145153023/a0d81d91-8f7c-4d86-92be-7f218db82319)

![Desktop Screenshot 2023 11 09 - 18 43 13 88](https://github.com/hipster-x/TOIB-3/assets/145153023/fa95370f-048c-453b-952f-75c1b361047f)

