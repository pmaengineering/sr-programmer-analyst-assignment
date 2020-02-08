# Assignment 1

## Description

At PMA we use [Open Data Kit](https://opendatakit.org) (not ODK-X) to collect data. One of the first things you will be asked to do is to learn this software so that you can help our data collection efforts.

The documentation for ODK is found [here](https://docs.opendatakit.org). I personally found [XLSForm.org](https://xlsform.org/en/) to be very useful in learning how to program questionnaires.

## Task

Create and convert an XLSForm of the questionnaire below. This requires using spreadsheet software, so Excel and Google Sheets are the most popular options.

### Questionnaire

1. How old are you?
2. Which activities do you enjoy? _Hint: Select all that apply_
  - Reading
  - Sports
  - Traveling
  - Cooking
  - None of the above
3. Have you graduated university?
  - Yes
  - No
4. In what month and year did you graduate university?

### Questionnaire notes

- Write the questionnaire so that all questions *require* an answer.
- Question (1) should accept an integer input. It should only allow numbers between 0 and 130.
- Question (2) should accept multiple choices. The choices are below it and above (3). Write logic so that "None of the above" cannot be selected with other options.
- Question (3) should only accept one choice. Its choices are "Yes" and "No".
- Question (4) should be asked only if question (3) is answered "Yes". Question (4) should be a date input and it should only accept month and year. Write logic so that the answer should not be in the future.

## Deliverable

You should share an `.xlsx` file and an `.xml` file with us. The `.xml` file should be created by converting the `.xlsx` file. These files should have the complete questionnaire above.

## Hints

- You will need a *survey* and a *choices* tab in your XLSForm.
- Use the online converter at [https://opendatakit.org/xlsform/](https://opendatakit.org/xlsform/) because it also lets you preview your questionnaire by clicking the "Preview in Enketo" button after submitting a file.
- The functions for questionnaire logic are defined in the docs [here](https://docs.opendatakit.org/form-logic/).

# Assignment 2

## Description

We have created the PMA API at [api.pma2020.org](http://api.pma2020.org) that others can use to get our data programmatically. It is not complete, but a subset of its functionality does work. We can get the data that we specify. Documentation can be found [here](http://api-docs.pma2020.org).

## Task

Your assignment is to write an app with a single screen that makes use of live data from PMA API.

Use the data from this query:
http://api.pma2020.org/v1/datalab/data?survey=PMA2014_BFR1&indicator=cp_all&characteristicGroup=edu_BF&overTime=false

And to get labels, combine with data from this query:
http://api.pma2020.org/v1/datalab/init

The labels can be found by doing the following. Compare the value for the key called `characteristic.label.id` in the `.../datalab/data` query (e.g. `IvgWGjvy`) to the `.../datalab/init` response.

For inspiration, see [DHS's mobile app](https://dhsprogram.com/data/mobile-app.cfm) and this screenshot from the app in particular:

![DHS mobile app screenshot](https://lh3.googleusercontent.com/j4ziAC6tUbaJidL8_krkZkfj-MmgCs8E-K_KLDLgjtcjsoUinV2SwE7USOIqqgVxid4=w3014-h2540)

This should showcase your talent with mobile app development. We would like to discuss this assignment during your in-person interview.

## Deliverable

You should share your codebase and be ready to discuss. We should be able to demo the app in-person.

## Beyond the task

Should you be hired, your work on this project (Assignment 2) would be a starting point for a mobile app to present our data. This could turn into something very popular with our donors and our partners.

# Help

I'm available as a resource for questions. Feel free to email or call. My contact information is in my email signature block.