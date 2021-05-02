# Araba_Database
This is a script written to work on dataframe extracted from Google sheet for my church's Database


Linking with google sheet
 1. we will link this notebook with the araba response google sheet , that way , we can easily perform all
    operations in real time without having to download and upload csv or excel files

 2. Also new tabs can be automatically created from here .
     we will be creating a tab called Contact details: this will be used by the media department to send 
     birthday sms to memebers 
     Also a tab called For analysis : this is to link with powerbi or tableau for analytics 
Cleaning the data
1. Names: First , middle and last name will be joined together to for FUll Names
         a. A column named Family will be Extracted

2. Dates: Date of birth and wedding anniversary will be converted into Datetime format
         a. Datetime will allow us exract info like Age so we cn group members according to their age

3. Geography: Because there is no consistence in how repondents fill thier state of origin , a code which 
   will filter unnecessary whitespace or info away from response will bw written 

4. Duplicates: all duplicates will be automatically removed with code

5. Blanks : cases where there are blanks (like society ) with be automatically filled with 'Non - Society'

6. Marital Status: there are cases where respondents filled marital status as Children , we will write a 
   code which automatically changes anything differnet from married or widowed to SIngle
