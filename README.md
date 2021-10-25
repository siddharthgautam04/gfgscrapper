# gfgscrapper


## About gfgextractor
Made a web scrapper which has ability to scrap the GeeksForGeeks website and save questions asked by companies in excel .
The purpose of this project is to extract information of question asked by different companies from GeeksForGeeks and present that information in the form of excel sheet. The application can be used
to solve real purpose problems of extracting large information from websites.

## TECH STACK USED
 -  JAVASCRIPT
 -  NPM Modules
    -  Minimist--> Takes command line arguments
    -  Axios--> For making http request <br>
    -  JSDOM--> For getting information from dom tree
    -  EXCEL4NODE--> Used to make excel filr
    -  PDF_LIB--> Used to make scorecards in the form of pds
    -  Puppeteer --> used for automation.
 
 ## FEATURES AND FUNCTIONS
 Dowloading data in the form of HTML by making a http request using axios as we are not using any browser so axios will help to achieve this.
 Reading HTML and extracting important and useful information using Jsdom
 Converting matches to teams using Array Manipulation
 Making of excel file and adding important stuff in that excel using excel4node library
 Making pdf and making changes to Template pdf using pdf-lib library.
 
 ## TO RUN THIS ON YOUR LOCAL
   First fork this to your profile, then clone it to your desktop
   
   Then install libraries 
   ```bash
  npm install minimist
  npm install axios
  npm install puppeteer
  npm install excel4node
  npm install jsdom
  
  ```
  
  To run this project use this command
  
  ```bash
   node gfg.js --excel=questions.csv --dataFolder=data --url="https://practice.geeksforgeeks.org/explore/?problemType=functional&difficulty%5B%5D=0&difficulty%5B%5D=1&difficulty%5B%5D=2&page=1&sortBy=submissions" 
  
  ```
## Code Summary
1. Read the command line arguments using minimist.

2. Read the HTML file use axios and convert it to DOM using JSDOM.

3. Using HTML elements and their class read the data which we need and push it into a JSO object.

4. Using the above JSO object with all match details we make another JSO which has team details using array manipulation.

5. Using the teams JSO and excel4node create an excel file with every team match details in a sheet.

6. Make folders using fs.



## CONTACT
In case of any suggestions or enquires, feel free to reach out to me at Sidgautam0104@gmail.com.
 
 

