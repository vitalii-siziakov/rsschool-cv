# CV - VITALII SIZIAKOV

* Location: Saint Petersburg, Russian Federation
* Date of birth: 25 January 1996

## CONTACTS

* Telegram: @vitalii_siziakov
* E-mail: vitalii.siziakov@gmail.com

## PROFILE

Dedicated to delivering effective solutions to all problems.  
Committed to utilizing my skills to help others.  
Hardworking and ready to quick learn.

## SKILLS

* HTML: Beginner
* CSS: Beginner
* JavaScript: Beginner
* PHP: Novice
* Git: Novice

## EDUCATION

* Bachelor of History at Institute of History, Saint Petersburg State University (September 2013 - June 2017)

## COURSES

* JavaScript. Professional Development of Web Interfaces at HTML Academy (May 2020 - July 2020)
* Learn Asynchronous JavaScript at Codecademy (December 2020)

## CODE EXAMPLES

* Create readble date (today)
```JavaScript
function createReadbleDateToday() {
    let dateToday = new Date();
    let yearToday = dateToday.getFullYear().toString();
    let monthToday = (dateToday.getMonth() + 1).toString();
    let dayToday = dateToday.getDate().toString();

    if (monthToday.length === 1) {
        monthToday = `0${monthToday}`;
    };

    if (dayToday.length === 1) {
        dayToday = `0${dayToday}`;
    };

    let result = `${yearToday}-${monthToday}-${dayToday}`;
    return result;
};                
```

* Convert number to number string with delimiters (spaces)
```JavaScript
function convertToNumberStringWithSpaces(numberWithoutSpaces) {
    if (numberWithoutSpaces === "") {
        return "0,00"
    } else {
        let delimiterIndex = numberWithoutSpaces.toString().indexOf('.');
        let firstPart = numberWithoutSpaces.toString();

        if (delimiterIndex !== -1) {
            let startIndex = 0;
            let endIndex = delimiterIndex;
            firstPart = numberWithoutSpaces.toString().substring(startIndex, endIndex);
        };

        firstPart = firstPart.toString().replace(/(\d)(?=(\d{3})+$)/g, '$1 ');

        let secondPart = `00`;

        if (delimiterIndex !== -1) {
            let startIndex = delimiterIndex + 1;
            let endIndex = delimiterIndex + 3;
            secondPart = numberWithoutSpaces.toString().substring(startIndex, endIndex);
        };

        if (secondPart.length === 1) {
            secondPart = `${secondPart}0`;
        };
        
        let result = `${firstPart},${secondPart}`;
        return result;
    };
};                  
```

## EMPLOYMENT HISTORY

* Specialist of the production and technical department at construction company NordInvest, LLC - Saint Petersburg, Russian Federation (Mart 2016 - January 2018)
* Car sales manager at Avtocentr, LLC - Saint Petersburg, Russian Federation (January 2018 - Present)

## LANGUAGES

* Russian: Native speaker
* English: A2
