## Hospital-Emergency-Room-Analysis | MS-Excel

### Data Loading
##### Load CSV File Into Excel -> Data -> Get Data -> Text/CSV -> Transform Data
##### This will take you to the Power Query Editor.

### Data Processing and Cleaning
#### 1. Merge Columns (Patient First Initital and Patient Last Name) to get new column (Patient Name)
#####   Select Both columns (Patient First Initital and Patient Last Name) -> Transform - > Merge Columns
#### 2. Replace values M to Male and F to Female in Patient Gender Column.
#####   Select Patient Gender -> Transform -> Replace Values
#### 3. Change data type of Patient Admission Flag to text and replace values False to Non-Admitted and True to Admitted.
#####   Select Patient Admission Flag -> Transform -> Replace Values
#### 4. Split Patient Admission Date into Patient Admission Date and Patient Admission Time.
#####   Transform -> Split Columns
#### 5  Make new Table Calendar_Date from Patient Admission Date by using Blank Query.
#####   Home - > New Source -> Other Sources -> then put formula - > = List.Dates(#date(2023,01,01),731,#duration(1,0,0,0))

####  Then go to close and load to option -> select only create connection and add this to data model model
####  Then go to Power Pivot Option -> Manange -> Create relation between Two tables by joining Date column of Calendar_date and Payment Admission Date of Hospital Emergency Room.

##### Then go to Data View in Manage Option and make two columns:-
##### 1. Age Group = =if([Patient Age]>70,"70-79",if([Patient Age]>60,"60-69",if([Patient Age]>50,"50-59",if([Patient Age]>40,"40-49",if([Patient Age]>30,"30-39",if([Patient Age]>20,"20-29",if([Patient Age]>10,"10-19","0-09")))))))
##### 2. Patient Attend Status = =if([Patient Waittime]>30,"Delay","Ontime")

