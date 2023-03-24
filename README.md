# Lab-5_202001426

## Name: Harshit Vadodia
## Student ID: 202001426
## IT314: Software Engineering

## Lab: 05 Static Analysis

### Theory

*Static Analysis:*
_Static analysis is a method of examining the source code of a software program without
executing it. Static analysis can help detect errors, bugs, vulnerabilities, and other quality issues
in the code. Static analysis tools can perform various tasks such as checking syntax, style,
logic, data flow, control flow, and security. Static analysis can improve the reliability,
performance, and maintainability of software by identifying and correcting defects early in the
development process._

*Static Analysis Tools:*
_Static analysis tools are software tools that analyze the source code of a program without
executing it. They can help developers find and fix errors, bugs, vulnerabilities, code smells, and
other quality issues in their code. Static analysis tools can also measure various metrics of the
code, such as complexity, readability, maintainability, test coverage, and documentation. Static
analysis tools can be integrated into the development process as part of the code editor, the
version control system, or the continuous integration pipeline. Some examples of static analysis
tools are SonarQube, PMD, ESLint, and Pylint._

### Link of github repository taken: hackstarsj/django-ecommerce-project-amazon-clone

### Tool used for Static Analysis: Pylint

#### Test 1: Analyzing error in the file admin.py in: https://github.com/hackstarsj/django-ecommerce-project-amazon-clone/tree/master/DjangoEcommerceApp

![image](https://user-images.githubusercontent.com/79862470/227486055-0bf016ea-83bd-49d1-afe7-dbe19ec51c4c.png)


### Error Analysis:

admin.py:6:0: C0304: Final newline missing (missing-final-newline)<br>
admin.py:1:0: C0114: Missing module docstring (missing-module-docstring)<br>
admin.py:1:0: E0401: Unable to import 'django.contrib' (import-error)<br>


#### Test 2: Analyzing errors in the file adminurls.py in: https://github.com/hackstarsj/django-ecommerce-project-amazon-clone/tree/master/DjangoEcommerceApp

![image](https://user-images.githubusercontent.com/79862470/227488108-fe4fed8d-1693-406e-8c7e-53d1d911d79a.png)

### Error Analysis

adminurls.py:33:0: C0303: Trailing whitespace (trailing-whitespace)<br>
adminurls.py:43:0: C0301: Line too long (110/100) (line-too-long)<br>
adminurls.py:48:0: C0301: Line too long (105/100) (line-too-long)<br>
adminurls.py:54:0: C0301: Line too long (109/100) (line-too-long)<br>
adminurls.py:55:0: C0301: Line too long (112/100) (line-too-long)<br>
adminurls.py:56:0: C0301: Line too long (110/100) (line-too-long)<br>
adminurls.py:57:0: C0301: Line too long (112/100) (line-too-long)<br>
adminurls.py:68:0: C0301: Line too long (105/100) (line-too-long)<br>
adminurls.py:70:0: C0304: Final newline missing (missing-final-newline)<br>
adminurls.py:16:0: E0401: Unable to import 'django.contrib' (import-error)<br>
adminurls.py:17:0: E0401: Unable to import 'django.urls' (import-error)<br>
adminurls.py:20:0: E0401: Unable to import 'django.conf.urls.static' (import-error)<br>
adminurls.py:20:0: C0411: third party import "from django.conf.urls.static import static" should be placed before "from DjangoEcommerceApp import views" (wrong-import-order)<br>
adminurls.py:22:0: C0411: third party import "from DjangoEcommerce import settings" should be placed before "from DjangoEcommerceApp import views" (wrong-import-order)adminurls.py:20:0: C0412: Imports from package django are not grouped (ungrouped-imports)<br>
adminurls.py:16:0: W0611: Unused admin imported from django.contrib (unused-import)<br>
adminurls.py:20:0: W0611: Unused static imported from django.conf.urls.static (unused-import)<br>
adminurls.py:22:0: W0611: Unused settings imported from DjangoEcommerce (unused-import)<br>


#### Test 3: Analyzing error in the file views.py in: https://github.com/hackstarsj/django-ecommerce-project-amazon-clone/tree/master/DjangoEcommerceApp

![image](https://user-images.githubusercontent.com/79862470/227492666-f6d87e7b-dbe8-4bef-8db1-d6290419a4a3.png)

### Error Analysis:

views.py:32:0: C0304: Final newline missing (missing-final-newline)       <br>
views.py:1:0: C0114: Missing module docstring (missing-module-docstring)  <br>
views.py:1:0: E0401: Unable to import 'django.shortcuts' (import-error)   <br>
views.py:2:0: E0401: Unable to import 'django.http' (import-error)        <br>
views.py:3:0: E0401: Unable to import 'django.contrib.auth' (import-error)<br>
views.py:4:0: E0401: Unable to import 'django.contrib' (import-error)<br>
views.py:5:0: E0401: Unable to import 'django.urls' (import-error)<br>
views.py:8:0: C0116: Missing function or method docstring (missing-function-docstring)<br>
views.py:8:0: C0103: Function name "demoPage" doesn't conform to snake_case naming style (invalid-name)<br>
views.py:8:13: W0613: Unused argument 'request' (unused-argument)<br>
views.py:11:0: C0116: Missing function or method docstring (missing-function-docstring)<br>
views.py:11:0: C0103: Function name "demoPageTemplate" doesn't conform to snake_case naming style (invalid-name)<br>
views.py:14:0: C0116: Missing function or method docstring (missing-function-docstring)<br>
views.py:14:0: C0103: Function name "adminLogin" doesn't conform to snake_case naming style (invalid-name)<br>
views.py:17:0: C0116: Missing function or method docstring (missing-function-docstring)<br>
views.py:17:0: C0103: Function name "adminLoginProcess" doesn't conform to snake_case naming style (invalid-name)<br>
views.py:22:4: R1705: Unnecessary "else" after "return", remove the "else" and de-indent the code inside it (no-else-return)<br>
views.py:29:0: C0116: Missing function or method docstring (missing-function-docstring)<br>
views.py:29:0: C0103: Function name "adminLogoutProcess" doesn't conform to snake_case naming style (invalid-name)<br>

#### Test 4: Analyzing error in the file models.py in: https://github.com/hackstarsj/django-ecommerce-project-amazon-clone/tree/master/DjangoEcommerceApp

![image](https://user-images.githubusercontent.com/79862470/227493279-03df60eb-1bd2-4deb-b9f1-522a5a2b457b.png)
![image](https://user-images.githubusercontent.com/79862470/227493361-03176b46-241d-42ab-81d3-4949dfa8b2c0.png)


### Error Analysis:

models.py:54:0: C0303: Trailing whitespace (trailing-whitespace)<br>
models.py:55:0: C0303: Trailing whitespace (trailing-whitespace)<br>
models.py:70:0: C0303: Trailing whitespace (trailing-whitespace)<br>
models.py:95:44: C0303: Trailing whitespace (trailing-whitespace)<br>
models.py:193:0: C0301: Line too long (104/100) (line-too-long)<br>
models.py:195:62: C0303: Trailing whitespace (trailing-whitespace)<br>
models.py:206:0: C0304: Final newline missing (missing-final-newline)<br>
models.py:1:0: C0114: Missing module docstring (missing-module-docstring)<br>
models.py:1:0: E0401: Unable to import 'django.db' (import-error)<br>
models.py:2:0: E0401: Unable to import 'django.contrib.auth.models' (import-error)<br>
models.py:3:0: E0401: Unable to import 'django.dispatch' (import-error)<br>
models.py:4:0: E0401: Unable to import 'django.db.models.signals' (import-error)<br>
models.py:5:0: E0401: Unable to import 'django.urls' (import-error)<br>
models.py:8:0: C0115: Missing class docstring (missing-class-docstring)<br>
models.py:8:0: R0903: Too few public methods (0/2) (too-few-public-methods)<br>
models.py:13:0: C0115: Missing class docstring (missing-class-docstring)<br>
models.py:13:0: R0903: Too few public methods (0/2) (too-few-public-methods)<br>
models.py:18:0: C0115: Missing class docstring (missing-class-docstring)<br>
models.py:18:0: R0903: Too few public methods (0/2) (too-few-public-methods)<br>
models.py:23:0: C0115: Missing class docstring (missing-class-docstring)<br>
models.py:23:0: R0903: Too few public methods (0/2) (too-few-public-methods)<br>
models.py:34:0: C0115: Missing class docstring (missing-class-docstring)<br>
models.py:34:0: R0903: Too few public methods (0/2) (too-few-public-methods)<br>
models.py:49:4: C0116: Missing function or method docstring (missing-function-docstring)<br>
models.py:58:0: C0115: Missing class docstring (missing-class-docstring)<br>
models.py:58:0: R0903: Too few public methods (1/2) (too-few-public-methods)<br>
models.py:73:0: C0115: Missing class docstring (missing-class-docstring)<br>
models.py:73:0: R0903: Too few public methods (0/2) (too-few-public-methods)<br>
models.py:88:0: C0115: Missing class docstring (missing-class-docstring)<br>
models.py:88:0: R0903: Too few public methods (0/2) (too-few-public-methods)<br>
models.py:97:0: C0115: Missing class docstring (missing-class-docstring)<br>
models.py:97:0: R0903: Too few public methods (0/2) (too-few-public-methods)<br>
models.py:107:0: C0115: Missing class docstring (missing-class-docstring)<br>
models.py:115:0: C0115: Missing class docstring (missing-class-docstring)<br>
models.py:115:0: R0903: Too few public methods (0/2) (too-few-public-methods)<br>
models.py:122:0: C0115: Missing class docstring (missing-class-docstring)<br>
models.py:122:0: R0903: Too few public methods (0/2) (too-few-public-methods)<br>
models.py:129:0: C0115: Missing class docstring (missing-class-docstring)<br>
models.py:129:0: R0903: Too few public methods (0/2) (too-few-public-methods)<br>
models.py:138:0: C0115: Missing class docstring (missing-class-docstring)<br>
models.py:138:0: R0903: Too few public methods (0/2) (too-few-public-methods)<br>
models.py:148:0: C0115: Missing class docstring (missing-class-docstring)<br>
models.py:148:0: R0903: Too few public methods (0/2) (too-few-public-methods)<br>
models.py:155:0: C0115: Missing class docstring (missing-class-docstring)<br>
models.py:155:0: R0903: Too few public methods (0/2) (too-few-public-methods)<br>
models.py:160:0: C0115: Missing class docstring (missing-class-docstring)<br>
models.py:160:0: R0903: Too few public methods (0/2) (too-few-public-methods)<br>
models.py:167:0: C0115: Missing class docstring (missing-class-docstring)<br>
models.py:167:0: R0903: Too few public methods (0/2) (too-few-public-methods)<br>
models.py:176:0: C0115: Missing class docstring (missing-class-docstring)<br>
models.py:176:0: R0903: Too few public methods (0/2) (too-few-public-methods)<br>
models.py:186:0: C0116: Missing function or method docstring (missing-function-docstring)<br>
models.py:186:24: W0613: Unused argument 'sender' (unused-argument)<br>
models.py:186:0: W0613: Unused argument 'kwargs' (unused-argument)<br>
models.py:198:0: C0116: Missing function or method docstring (missing-function-docstring)<br>
models.py:198:22: W0613: Unused argument 'sender' (unused-argument)<br>
models.py:198:0: W0613: Unused argument 'kwargs' (unused-argument)<br>

#### Test 5: Analyzing error in the file tests.py in: https://github.com/hackstarsj/django-ecommerce-project-amazon-clone/tree/master/DjangoEcommerceApp

![image](https://user-images.githubusercontent.com/79862470/227493558-44ee300d-0aae-4918-8cd2-92b215423aee.png)

tests.py:1:0: C0114: Missing module docstring (missing-module-docstring)<br>
tests.py:1:0: E0401: Unable to import 'django.test' (import-error)<br>
tests.py:1:0: W0611: Unused TestCase imported from django.test (unused-import)<br>
