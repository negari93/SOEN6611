# SOEN6611

File Structure of the Repository

I) Folder "CodeCoverage" contains raw data regarding Statement Coverage and Branch Coverage produced by JaCoCo. Subfolders are divided by projects' name.
II) Folder "Mutation Testing" contains raw data for mutation testing
III) Folder "McCabe" contains raw data for McCabe cyclomatic complexity.
IV) Folder "CodeChurn" contains raw data collected for code churn as fifth metric
VI) Folder "Findbugs" contains raw data collected for static analysis.


Requirements:

1- Intellij IDEA it has JaCoCo as a built in plugin. JaCoCo has been used for both metrics 1 and 2.
2- PIT plugin needs to be installed to perform mutation testing.
3- Tool for McCabe 
4- Cloc open source software available on GitHub. Version used in our experiment is 1.80. It can be downloaded via link below:
https://github.com/AlDanial/cloc/releases 
5- Finbugs plugin offered by Intellij IDEA to collect data for sixth metric

Team Members:

Balpreet Singh	40070817

Kritika Saini	40049120

Negar Sadeghi	40028394

Shubham Sagar	40089224

Subhodip Ray	40080104


Configurations in order to get data for each metric:

1- Code Coverage: We have used JaCoCo which is a build in plug in in Intellij IDEA.
1.a Select the project, from "Run" select "Edit Configuration" then click on + to add a new configuration. Select Junit as your test configuration. Tesk kind should be chosen as "All in package". Then prefered package has to be chosen. Intellij will automaticaly detect required module, in case a no module found error appears you need to select projects module. On the "Code Coverage" tab select JaCoCo and then add package to perform the coverage on.
2- Make sure that for Intellij check if SDK 1.8 is imported. This can be checked from File -> Project Structure -> Project -> Project SDK and choose 1.8. Also select Project language level as 8- Lambdas, type annotations etc.
3- Junit.jar file has to be added to project settings: File -> Project Structure -> Modules -> Dependencies if no Junit.jar file is added by default you need to look for it in the place you have downloaded it and add it to dependencies. Scope of this jar file is test.
