XML
 1. Создать внешний репозиторий c названием XML. ----- + -> new repository -> заполнить поле "Repository name" -> чек бокс "Add a README file" -> кликнуть кнопку "create repository"
 2. Клонировать репозиторий XML на локальный компьютер. ----- git clone https://github.com/Pavlik1100/XML.git  
 3. Внутри локального XML создать файл “new.xml”. ----- touch new.xml
 4. Добавить файл под гит. ----- git add new.xml
 5. Закоммитить файл. ----- git commit -m "created file new.xml"
 6. Отправить файл на внешний GitHub репозиторий. ----- git push  
 7. Отредактировать содержание файла “new.xml” - написать информацию о себе (ФИО, возраст, количество домашних животных, будущая желаемая зарплата). Всё написать в формате XML. -----  

vim new.xml  
  
------
  
<?xml version="1.0" encoding="UTF-8" ?>  
  
<FIO>SimonovPavelSergeevich</FIO>  
<age>28</age>  
<count_pets>0</count_pets>  
<salary>1000</salary>  
  

 8. Отправить изменения на внешний репозиторий.  -----  
  
git add new.xml  
git commit -m "update new.xml"  
git push 

 9. Создать файл preferences.xml ----- > preferences.xml  
 10. В файл preferences.xml добавить информацию о своих предпочтениях (Любимый фильм, любимый сериал, любимая еда, любимое время года, сторона которую хотели бы посетить) в формате XML. -----  
  
vim preferences.xml  
  
-----  
  
<?xml version="1.0" encoding="UTF-8" ?>  
  
<favourite_film>Blade_runner</favourite_film>  
<favourite_serial>LOST</favourite_serial>  
<favourite_food>fried_chiken</favourite_food>    
<favourite_time_of_the_year>summer</favourite_time_of_the_year>  
<next_visit_country>USA</next_visit_country>    


 11. Создать файл sklls.xml добавить информацию о скиллах которые будут изучены на курсе в формате XML -----  

> skills.xml  
vim sklls.xml  
  
-----  
<?xml version="1.0" encoding="UTF-8" ?>  

<skill_1>why_QA</skill_1>    
<skill_2>when_QA</skill_2>    
<skill_3>where_QA</skill_3>    


 12. Сделать коммит в одну строку. -----  
 
Так как файлы только созданы и небыли git add то добавление и коммит в одной строке не выйдет. Однако при следующем изменении добавить и закомитить можно будет одной строкой.
  
 git add prefereces.xml skills.xml  
 git commit -m "added files preferences.xml skills.xml"  


 13. Отправить сразу 2 файла на внешний репозиторий. ----- git push  
 14. На веб интерфейсе создать файл bug_report.xml. ----- add new file -> заполнить поле названия файла   
 15. Сделать Commit changes (сохранить) изменения на веб интерфейсе. ----- добавить commit в поле "commit changes" -> отметить чекбокс "commit directory to the main branch" -> нажать кнопку "commit changes"
 16. На веб интерфейсе модифицировать файл bug_report.xml, добавить баг репорт в формате XML. ----- выбрать в дериктории файл для редактирования, кликнуть чтобы открыть -> нажать кнопку с карандашом "Edit this file" -> ввести данные в формате XML  

<?xml version="1.0" encoding="UTF-8" ?>   
    
<Title>Button_'Home'_dont_click</Title>  
<Steps>Open_web_and_click_button_'Home'</Steps>  
<Facual_result>When_button_click_nothing_is_happening</Facual_result>  
<Expected_result>When_button_click_we_back_home_page</Expected_result>  
<Severity>Medium</Severity>  
  

 17. Сделать Commit changes (сохранить) изменения на веб интерфейсе. ----- добавить commit в поле "commit changes" -> отметить чекбокс "commit directory to the main branch" -> нажать кнопку "commit changes"
 18. Синхронизировать внешний и локальный репозиторий XML  ----- git pull