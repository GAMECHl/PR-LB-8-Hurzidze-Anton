## Хурцидзе Антон IПЗ 3.02 Практична-Лабораторна робота № 8

## Тема: Неперервна інтеграція
## Мета: ознайомитися з принципами і практиками неперервної інтеграції, сформувати навички автоматизації CI/CD процесів в GitHub Actions

## 1) Починаємо першу практичну роботу на GitHub Skills за наступним посиланням https://github.com/skills/hello-github-actions?tab=readme-ov-file

#### 1. Переходимо за посиланням та натискаємо на кнопку ``Start course`` та створюємо репозиторій:
![1](https://github.com/GAMECHl/PR-LB-8-Hurzidze-Anton/blob/main/1.png)
#### Рис. 1 - Створення репозиторія

#### 2. Переходимо на сторінку ``Pull requests``, натискаємо на створення нового Пулл запиту та налаштовуємо запит наступним чином:
![2](https://github.com/GAMECHl/PR-LB-8-Hurzidze-Anton/blob/main/2.png)
![3](https://github.com/GAMECHl/PR-LB-8-Hurzidze-Anton/blob/main/3.png)
#### Рис. 2 - Створення пулл запиту

#### 3. Переходимо на сторінку ``Code``, натискаємо на гілку та обираємо нову створену гілку ``welcome-workflow``:
![4](https://github.com/GAMECHl/PR-LB-8-Hurzidze-Anton/blob/main/4.png)
#### Рис. 3 - Переход на нову гілку

#### 4. Переходимо в папку ``.github/workflows``, створюємо новий файл ``welcome.yml`` та додаємо в нього наступний зміст:
![5](https://github.com/GAMECHl/PR-LB-8-Hurzidze-Anton/blob/main/5.png)
#### Рис. 4 - Створення файла welcome.yml

#### 5. Натискаємо на кнопку ``Commit changes`` та підтверджуємо створення нового файлу, впевневшись що ми коммітимо цей файл в корректну гілку ``welcome-workflow``:
![6](https://github.com/GAMECHl/PR-LB-8-Hurzidze-Anton/blob/main/6.png)
#### Рис. 5 - Підтвердження створення файлу

#### 6. Чекаємо пів хвилини та перезавантажуємо сторінку, зміст сторінки readme змінется, потім відкриваємо файл ``welcome.yml`` та змінюємо його зміст наступним чином:
![7](https://github.com/GAMECHl/PR-LB-8-Hurzidze-Anton/blob/main/7.png)
#### Рис. 6 - Додавання роботи файлу welcome.yml

#### 7. Чекаємо пів хвилини, відкриваємо файл ``welcome.yml`` та знову змінюємо його зміст наступним чином:
![8](https://github.com/GAMECHl/PR-LB-8-Hurzidze-Anton/blob/main/8.png)
#### Рис. 7 - Додавання шагу файлу welcome.yml

#### 8. Потім натискаємо на сторінку ``Pull requests``, потім на створенний запит із другого пункта і потім на кнопку ``Merge pull request`` та підтверджуєм:
![9](https://github.com/GAMECHl/PR-LB-8-Hurzidze-Anton/blob/main/9.png)
#### Рис. 8 - Сливання гілок

#### 9. Опціонально видаляємо гілку ``welcome-workflow``:
![10](https://github.com/GAMECHl/PR-LB-8-Hurzidze-Anton/blob/main/10.png)
#### Рис. 9 - Видалення не потрібної гілки

## 2) Починаємо другу практичну роботу на GitHub Skills за наступним посиланням https://github.com/skills/hello-github-actions?tab=readme-ov-file

#### 1. Переходимо за посиланням та натискаємо на кнопку ``Start course``, створюємо репозиторій:
![11](https://github.com/GAMECHl/PR-LB-8-Hurzidze-Anton/blob/main/11.png)
#### Рис. 10 - Створення репозиторія

#### 2. Переходимо на сторінку ``Code``, потім на гілку ``cd``, потім в директорію ``.github/workflows/``:
![12](https://github.com/GAMECHl/PR-LB-8-Hurzidze-Anton/blob/main/12.png)
#### Рис. 11 - Переход в гілку та в директорію

#### 3. Створюємо файл ``publish.yml``, з наступним змістом:
![13](https://github.com/GAMECHl/PR-LB-8-Hurzidze-Anton/blob/main/13.png)
#### Рис. 12 - Створення файла publish.yml

#### 4. Переходимо на сторінку ``Pull requests``, натискаємо на створення нового Пулл запиту та налаштовуємо запит наступним чином:
![14](https://github.com/GAMECHl/PR-LB-8-Hurzidze-Anton/blob/main/14.png)
#### Рис. 13 - Створення пулл запиту

#### 5. В гілці ``cd`` створюємо ``Dockerfile`` з наступним змістом:
![15](https://github.com/GAMECHl/PR-LB-8-Hurzidze-Anton/blob/main/15.png)
#### Рис. 14 - Створення Dockerfile

#### 6. Потім натискаємо на сторінку ``Pull requests``, потім на створенний запит із четвертого пункта і потім на кнопку ``Merge pull request`` та підтверджуєм(опціонально видаляєм гілку ``cd``):
![16](https://github.com/GAMECHl/PR-LB-8-Hurzidze-Anton/blob/main/16.png)
#### Рис. 15 - Сливання гілок

#### 7. Запускаємо ``Docker Desktop for Windows``:
![18](https://github.com/GAMECHl/PR-LB-8-Hurzidze-Anton/blob/main/18.png)
#### Рис. 16 - Запуск докера

#### 8. Генеруємо токен в налаштуваннях свого гітхабу:
![19](https://github.com/GAMECHl/PR-LB-8-Hurzidze-Anton/blob/main/19.png)
#### Рис. 17 - Генерування токену

#### 9. Прописуємо команду docker login ghcr.io -u USERNAME та потім вставляємо згенерований токен:
![20](https://github.com/GAMECHl/PR-LB-8-Hurzidze-Anton/blob/main/20.png)
#### Рис. 18 - Логін в докер

#### 10. Потім прописуємо команду docker pull ghcr.io/YOURNAME/publish-packages/game:TAG та дивимся на результат:
![17](https://github.com/GAMECHl/PR-LB-8-Hurzidze-Anton/blob/main/17.png)
#### Рис. 19 - Пулл image

#### 11. Для находження інформації про ``image`` треба прописати наступну команду:
![21](https://github.com/GAMECHl/PR-LB-8-Hurzidze-Anton/blob/main/21.png)
#### Рис. 20 - Інформація про image

#### 12. Потім запускаємо наступну команду docker run -dp 8080:80 --rm <YOUR_IMAGE_NAME:TAG> для запуску контейнера з image:
![22](https://github.com/GAMECHl/PR-LB-8-Hurzidze-Anton/blob/main/22.png)
#### Рис. 21 - Запуск контейнера

#### 13. Перейдемо в докер та побачимо наш запущенний контейнер:
![23](https://github.com/GAMECHl/PR-LB-8-Hurzidze-Anton/blob/main/23.png)
#### Рис. 22 - Запущений контейнер

#### 14. Та перейдемо на сторінку http://localhost:8080/ та побачимо результат наших дій:
![24](https://github.com/GAMECHl/PR-LB-8-Hurzidze-Anton/blob/main/24.png)
#### Рис. 23 - Сторінка http://localhost:8080/

## 3) Створення власного Workflow

#### 1. Відкриємо фронт-енд проект із лабораторної роботи №6 та запушимо його наступним чином:
![25](https://github.com/GAMECHl/PR-LB-8-Hurzidze-Anton/blob/main/25.png)
![26](https://github.com/GAMECHl/PR-LB-8-Hurzidze-Anton/blob/main/26.png)
#### Рис. 24 - Пуш фронт-енду

#### 2. Відкриємо сторінку створенного гітхабу та подивимось на результат:
![27](https://github.com/GAMECHl/PR-LB-8-Hurzidze-Anton/blob/main/27.png)
#### Рис. 25 - Запушений фроент-енд

#### 3. Створемо каталог ``.github``, в ньому каталог ``workflows``, і в ньому файл ``docker-build.yml`` з наступним змістом:
![28](https://github.com/GAMECHl/PR-LB-8-Hurzidze-Anton/blob/main/28.png)
#### Рис. 26 - Файл docker-build.yml

#### 4. Перейдемо на сторінку ``Actions`` і побачимо що все працює корректно:
![29](https://github.com/GAMECHl/PR-LB-8-Hurzidze-Anton/blob/main/29.png)
#### Рис. 27 - Результат роботи файлу docker-build.yml

#### 5. Перейдемо на свій профіль та на сторінку ``Packages`` і побачимо що з'явився докер екземпляр:
![30](https://github.com/GAMECHl/PR-LB-8-Hurzidze-Anton/blob/main/30.png)
#### Рис. 28 - Сторінка Packages в гітхабі

## Висновки: Протягом виконання лабораторно-практичної роботи я ознайомився з принципами і практиками неперервної інтеграції та сформував навички автоматизації CI/CD процесів в GitHub Actions
