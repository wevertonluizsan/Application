\# criar uma aplicação e clonar



cd C:\\ExemploConflict\\GitMerge And Conflict\\Developer A

git clone https://github.com/wevertonluizsan/Application.git



cd C:\\ExemploConflict\\GitMerge And Conflict\\Developer B

git clone https://github.com/wevertonluizsan/Application.git





=======================



\# modificar o arquivo readme



cd **C:\\ExemploConflict\\GitMerge And Conflict\\Developer A\\Application**



**git branch developera**



**git checkout developera**



**git add .**



**git commit -m "Developer A story change"**



**git checkout main**



**git merge developera**



**git push origin main**







**===================**





cd **C:\\ExemploConflict\\GitMerge And Conflict\\Developer B\\Application**

**git branch developerb**

**git checkout developerb**

**git add .**

**git commit -m "Developer B story change"**

**git checkout main**

**git merge developerb**

git push origin main



\# acima deu erro por causa de conflito o pull da oportunidade de localizar os conflitos e resolver



git pull



**# ir no arquivo e abrir e resolver os conflitos**



**git add .**



**git commit -m "Developer B story"**

**git push origin main**







