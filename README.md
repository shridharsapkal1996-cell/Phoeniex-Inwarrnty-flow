# Postman API Automation integration with Github action #
This repository is a demonstration for POC for integrating postman tests with github actions. The Tests are written in Postman and they are executed on the VM with the help of newman and newman-reporter-htmlextra.
Github Actions will trigger the project execution on every push to the main brach.You can also execute project manualy using workflow_dispatch.The project run on a schedule time with the help on cron job.

The HTMP report archive in the artifact section for the team to download it.Along with that they can view the report directly from the github page : https://shridharsapkal1996-cell.github.io/Phoeniex-Inwarrnty-flow/
The latest repot mail to the team members using GMAIL SMTP.

## Testing coverage ##
1-Happy flow testing 
2-Negative testing and edge coverage testing 
3-token testing 
4-data driven testing with csv
5-schema validation 
6-screte managemnet with github screate 

## Tech Stack ##
1-Postman
2-Nodejs 22v
3-Newman 
4-newman-reporter-htmlextra
5-github-action
6-gmail-SMTP
7-Github-pages 
8-CSV for data driven testing 
9-AWS-EC2 instance for self hosted runner.

## Github pages ##
You can directly view the latest test report of the postman test on the link :https://shridharsapkal1996-cell.github.io/Phoeniex-Inwarrnty-flow/

## HTML report ##
The report will be created in the newman folder 
![Postman_report](https://shridharsapkal1996-cell.github.io/Phoeniex-Inwarrnty-flow/)

## Project structure ##
Phoenix Inwarrenty Flow
├─ Inwarranty-Flow-Request Copy.postman_collection.json #Collection
├─ newman                                               #Report
│  ├─ Inwarranty-Flow-Request Copy-2026-02-08-16-54-29-498-0.html
│  ├─ Inwarranty-Flow-Request Copy-2026-02-08-17-32-24-294-0.html
│  ├─ Inwarranty-Flow-Request Copy-2026-02-10-17-41-02-687-0.html
│  ├─ newman-run-report-2026-02-08-16-33-06-671-0.html
│  ├─ newman-run-report-2026-02-08-16-54-29-498-0.html
│  └─ newman-run-report-2026-02-08-17-32-24-292-0.html
├─ QA INT.postman_environment.json   
├─ textdata.csv                        #Testdata
└─ workspace.postman_globals.json

## How to run the project ##
You can run the project on local system for that :
1-Clone the project in your local system:https://github.com/shridharsapkal1996-cell/Phoeniex-Inwarrnty-flow.git
2-Install node.js and npm from :https://nodejs.org/en
3-Install newman using next command npm install -g newman
4-Install newman reporter with this command:npm install -g newman-reporter-htmlextra
5-Run the newman command 
 newman run "Inwarranty-Flow-Request Copy.postman_collection.json" \
          -e "QA INT.postman_environment.json" \
          -d "textdata.csv" \
          -r cli,htmlextra \
          --reporter-htmlextra-export ./newman/index.html

## About Me ## 
Hi my name is shridhar I have 4 years of the experience in automation testing and devops my skillsets are including the UI automation with selenium ,cypras,cucumber,playwrite and for the API testing ,Reach out to me the Likned in profile https://in.linkedin.com/


