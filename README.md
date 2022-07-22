# BabyBus Money+
The Utilization of ScalarDB on Bank Transaction System: A database assignment.
<br> Team: BabyBus
<br> Members: Junjie GAO, Shengze WANG, Danyuan YU, Xiang MENG, Jingyu LIU
## Introduction to the repository
The repository includes two files, which are a PDF file and a pptx file. The pptx file includes the slide that we used for the final presentation and the PDF file includes a link to download the Zip file. 
## Requirements
- Docker
- Gradle (7.4.2)

## Databases
- MySQL

## Operation methods
1. set up Docker.
`money-transaction-system-app % docker-compose up`
2. run the command below together with step 1．
`money-transaction-system-app % ./gradlew build`
3. Create the table written in schema.json in the same tab as 2.
`java -jar tools/scalardb-schema-loader-3.5.2.jar --config app/src/main/resources/database.properties --coordinator -f tools/schema/schema.json`
4. Start the server in the same tab as 2.
`money-transaction-system % gradle run`

## This should be the proper procedure of running the app, but it is still possible that the code failed to run. 
To cope with potential accidents, we packed our code to .exe file which should be easier to run. 
1. Open the PDF file to access the Google Drive to download our Zip file.
2. Download the Zip file from our github.
3. Unfreeze the Zip file.
4. Find the /dist folder.
5. server2.exe is located in the above folder.

## Appendix
We have two reasons to wrap into .exe file. First, it is easy for you to check our system. Second, we used cloud server but we can not make our password public.
<br> Test ID: bank_Gao
<br> Password: 123456
