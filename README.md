# My capstone case studies for the Google Data Analytics Certificate

During some free time at university, I enrolled in the [Google Data Analytics Professional Certificate on Coursera](https://www.coursera.org/professional-certificates/google-data-analytics?utm_source=gg&utm_medium=sem&utm_campaign=15-GoogleDataAnalytics-ROW&utm_content=15-GoogleDataAnalytics-ROW&campaignid=12566515400&adgroupid=117869292845&device=c&keyword=google%20data%20certification&matchtype=b&network=g&devicemodel=&adpostion=&creativeid=507290840621&hide_mobile_promo&gclid=CjwKCAjwieuGBhAsEiwA1Ly_nW0b8kYk9covlwaMOn7AAHj-pwimBJu1BJoDXrcxvuykE_Vm3paHGRoCdfYQAvD_BwE) to sharpen my skills with data analytics tools that I want to use. In the process, I was greeted by a collection of instructors that each handed me the start of a thread that lead deeper into the tapestry of analytics. 

<p align="center">
  <img width="825" src="https://github.com/nuclearcheesecake/wickusgoogledataanalyticscertificate2021/blob/main/Misc/course.png">
</p>

This is due to the course having a strong focus on the methodology of data analytics projects, with each phase representing an area of expertise to explore. The phases that Google suggests are:

* Ask, or a preliminary analysis of the scenario (stakeholder and problem analyses)
* Prepare, or collecting and storing data for our specific analysis and testing its bias and credibility
* Process, or cleaning and preparing the data for analysis
* Analyse, or finding patterns and generating insights using the data
* Share, or creating visualisations and presentations
* Act, or taking action with stakeholders given the new insights

To complete the certificate, I had to design and complete a case study that implements this methodology, as was taught in the course. I had three options for the case study, but, in the interest of gaining more practice with my data analytics tools, I decided that all three are good applications to explore. Thus in this repositiory, you will find the following three case studies that I have completed using the methodology above:

1. [Developing a new marketing strategy to increase influx of annual memberships at a bike-sharing company (with a focus on **Microsoft Excel** and **R**)](#case1)
2. [Guide a marketing strategy based on how users interact with fitness smart devices (with a focus on **SQL**)](#case2)
3. [Case study 3 (with a focus on **R**)](#case3)

The first two are theoretical case studies created by Google, and thus all the data was provided by them. For the last option, however, I had to find an alternative data source. Here follows my three case studies. As stated above, these case studies will implement the Google Data Analytics methodology. To further test out my toolset, I decided to attempt all 3 case studies with a primary focus on a singular tool (stated boldly in brackets above).

<a name="case1"></a>
## Case Study 1 - Developing a new marketing strategy to increase influx of annual memberships at a bike-sharing company

<p align="center">
  <img width="310p" src="https://github.com/nuclearcheesecake/wickusgoogledataanalyticscertificate2021/blob/main/Misc/carl-nenzen-loven-igKjieyjcko-unsplash.jpg">
</p>

(For the scenario supplied by Google, see [here](https://github.com/nuclearcheesecake/wickusgoogledataanalyticscertificate2021/blob/main/Case%20study%201/case1.pdf).)

### Step 1 - Initial scenario investigation 👔

In this scenario, I am a junior data analyst working for the marketing analyst team at **Cyclistic**, a company in Chicago with a bike-sharing program that is important to its operation. This team now has the goal of guiding the future marketing program, and I was tasked with a specific question to answer:

*How do annual members and casual rides use Cylistic bikes differently?*

At the end of my analysis, I am expected to hand in a report summarising all the steps I took, and my recommendations for a marketing campaign. I will be using this space on GitHub to jot down my thoughts in the process of answering this question - but if you are interested only in the final deliverable, click HERE.

As explained in the introduction above, I will focus on using **Microsoft Excel** in this case study.


* **The stakeholders and important players in this project**

**Lily Moreno** - director of marketing and my manager - she believes that maximising number of annual memberships will dicate company's future success. She is also respinsible for the development of campaigns and initiatives to promote the program.

**Cyclistic executive team** - the higher-ups who are detail-oriented and will decide to approve the recommended marketing campaign. They are also the people who are most interested in the success of the company.

**Casual rider** - person with a single-ride or a full-day pass - aware of program and chose it for mobility needs.

**Cyclistic members** - person with an annual membership - believed to be more profitable than casual riders.


* **What problem am I trying to solve?**

The goal of this project is to create a marketing campaign to convert casual riders into members, since this will be more profitable for the company. Thus we are not focusing on gaining new people into the program, but rather on how we can convince existing people who are casual riders to upgrade to annual memberships.

To do this, I will solve the problem of how they use the program differently than members.

From this description of the problem I can generate the business task, since in the end we are interested in finding out *how we can get more people to sign up for annual memberships*, as this will increase revenue for the company.


* **How can my insights drive business decisions?**

Finding out how these two groups of users differ, will hopefully show us how to market towards the casual riders to show them how an annual membership can benefit their needs. They might not be aware of the benefit, and will be able to use the program more effectively once upgraded.
<br/><br/>

### Step 2 - Obtaining the correct data 📜

For this project, I will use data from June 2020 to May 2021, as this is the most recent data available at the time of analysis (July 2021). The data for this project is located in a [public data source](https://divvy-tripdata.s3.amazonaws.com/index.html). 

* **Storing and organising the data**

During my analysis, the data will be stored on my private computer, in the following folder:

<p align="center">
  <img width="825" src="https://github.com/nuclearcheesecake/wickusgoogledataanalyticscertificate2021/blob/main/Misc/cs1_data.png">
</p>

The filepath for this folder is *C:\Users\wicka\Desktop\Google Data Analytics certification\Course 8 - Capstone project - Complete a case study\Case Study 1\Data used (pre-processed)*. 
As can be seen above, the data is organised according to **yearmonth_name.csv**. These are thus all .csv files, which is rather nice, since I can import them to most tools of my choice.

I am keeping a copy of the raw, unprocessed data in the folder above as a backup. I will work with the data after importing it to an Excel filed located in a folder called *Data used (working)*. Each sheet represents a different month, as can be seen here:

<p align="center">
  <img width="825" src="https://github.com/nuclearcheesecake/wickusgoogledataanalyticscertificate2021/blob/main/Misc/cs1_excel.png">
</p>

* **Bias and credibility**

Since data has been collected on both casual riders and members, it is not skewed towards one. We have data about the whole population - quite a unique situation! 

We can further use the ROCCC analysis as suggested by the course to see if the data is unbiased:

- Reliable ✔️ - We are using the company's own data
- Original ✔️ - Data used is internal, original copies
- Comprehensive ✔️ - Contains enough attributes on cyclist info to be useful
- Current ✔️ - We obtained data from the last 12 months
- Cited ✔️ - We are using the company's own data

Thus we can say that the data we have gathered is certain to be unbiased. The results obtained can thus be seen as credible.


* **Licensing, privacy, security and accessibility**

The data can be used with the following [license](https://www.divvybikes.com/data-license-agreement).

As it is a requirement of creating a schema in SQL Developer, the database automatically is password-protected. But since I am on a private network with an anti-virus, and the data is just dummy data, this step is not all that necessary. 

The data, in its raw form, can be accessed [here](https://divvy-tripdata.s3.amazonaws.com/index.html). 12 files are relevant to this study - download the zip files from June 2020 to May 2021.

* **Verifying the data's integrity**

The data was generated in-house by the company, but there seems to be a lot of missing values in certain columns. How this affects the analysis will be explored when the data is cleaned.  Replication errors won't be taken into account, since the data is sourced from the central database in the company, and the data engineers will have taken care to keep a safe original copy of the data, and furthermore protect the data from viruses.

We can thus assume that the data has good integrity.

* **How will the data help me answer the proposed question?**

Now that the data has been loaded, and after it has been cleaned, I can use it to figure out user's preferences with the bikes, and if those preferences form trends depending on which type of rider they are. I see that there are electric bikes, docked bikes and classic bikes, which could be a nice attribute to explore. I can also explore the frequency of use, and peak times of use, and if different riders have different peak riding times. Another interesting quantity to explore is the distance that riders travel on average.

* **Problems found with the data**

As mentioned previously, the data seems to have a lot of missing values that will be dealt with in the next step. 

Since the whole population was chosen, there is a very large amount of entries in the database, which could cause Excel to be overworked. I am considering moving the data to SQL, but for now Excel seems to handle the strain well, and I want to use Excel for this case study. The slowness of operations might decrease my efficiency, but we will deal with that if it becomes a problem.
<br/><br/>

### Step 3 - Cleaning and processing the data 🧹️
To ensure the integrity of the original data, I imported the data into Excel, where it will be processed. This ensures that the original data is not altered in my investigation. 
* **Calculated rows**
For each sheet, the following two columns were added:
<p align="center">
  <img width="825" src="https://github.com/nuclearcheesecake/wickusgoogledataanalyticscertificate2021/blob/main/Misc/cs1_weekday.png">
</p>

**The duration of the ride (ride_length)**

This was done by subtracting the time started from the time ended, and then formatting the row as HH:MM:SS using built-in Excel commands.

**The day of the week (day_of_week)**

By using the WEEKDAY() function, where 1 = Sunday and 7 = Saturday, on the day that the ride started.

* **Dealing with missing data**

The large amount of empty entries I saw in the previous phase are now seen to be the station ID and station name of the places where the bikes are fetched and dropped off. These columns are not essential to our study, and can thus be deleted since the stations names and IDs can be obtained from the original files if they are needed. And with further consideration, I have decided to delete the remaining positional data (the latitude and longtitude) of the start and end station as well. My logic will all these deletions are that I have calculated ride_length which is a metric that we can observe user engagement with, and the straight-line distance tha could be calculated with the locational data between start and end wouldn't tell us much more anyway. In other words, distance and time of travel both tell us basically the same thing - how much the user engages with the service, and time is the better metric, so we can remove distance to keep the analysis elegant.

Now for missing data in the remaining columns - for this, we will use conditional formatting. For each sheet, I added a rule to highlight cells in a different colour if their value is empty. With this method I was able to scroll through the data and easily spot where there was open cells missing data. There was no data missing in the columns left in the spreadsheet. Afterwards, I deleted the conditional formatting rules again.

<p align="center">
  <img width="825" src="https://github.com/nuclearcheesecake/wickusgoogledataanalyticscertificate2021/blob/main/Misc/cs1_formatting.png">
</p>

* **Checking for entry errors**

First, I checked the obvious categories which only has a finite number of values from a selection - the type of bike and the type of member. For this I used the UNIQUE() function to see if there are any values in these columns that do not fall in one of the categories, for example if someone misspelled one of the category names. No such errors were found.

<p align="center">
  <img width="825" src="https://github.com/nuclearcheesecake/wickusgoogledataanalyticscertificate2021/blob/main/Misc/cs1_entry.png">
</p>

I also then sorted each sheet according to ride_length, since this is the other column that would cause chaos if entires were made erroneously in the start/end columns. By sorting, I can see if there is a value at the top of bottom that stands out as an error. And indeed there are values which needs some attention, manifesting as a series of X's. Upon further investigation, these X's are in rows where the end time is before the start time.

<p align="center">
  <img width="825" src="https://github.com/nuclearcheesecake/wickusgoogledataanalyticscertificate2021/blob/main/Misc/cs1_errors.png">
</p>

This was fixed by changing the criteria of ride_length to:

```
=IF([@[ended_at]] >[@[started_at]]; [@[ended_at]] - [@[started_at]]; [@[started_at]] - [@[ended_at]])
```

* **Removing duplicates**

For this, Excel provided me with an easy option. I just selected the "Remove Duplicates" button, and voila!

<p align="center">
  <img width="825" src="https://github.com/nuclearcheesecake/wickusgoogledataanalyticscertificate2021/blob/main/Misc/cs1_duplicates.png">
</p>

No duplicates were found in any of the sheets.

Now that our data has been cleaned and saved in a usable format, we can start our analysis.

<br/><br/>

### Step 4 - Analysis 🕵️‍♂️

After waiting more than 10 minutes for Excel to sort a single sheet, I decided to do my analysis in R, since that will save me a lot of time. Thus I begin by converting all 12 sheets to seperate .csv files (and numbering them 1 through 12), and then importing them to R. For this analysis, I will be using the RStudio IDE. 

First, we load the data into R. After that we can combine the 12 data frames into 1 to see data for the whole year, such as how many of each type of rider there is.

```
data_202006 = read.table(file = "C:\\Users\\wicka\\Desktop\\Google Data Analytics certification\\Course 8 - Capstone project - Complete a case study\\Case Study 1\\Data used (working)\\1.csv", header = T, sep = ";")
data_202007 = read.table(file = "C:\\Users\\wicka\\Desktop\\Google Data Analytics certification\\Course 8 - Capstone project - Complete a case study\\Case Study 1\\Data used (working)\\2.csv", header = T, sep = ";")
data_202008 = read.table(file = "C:\\Users\\wicka\\Desktop\\Google Data Analytics certification\\Course 8 - Capstone project - Complete a case study\\Case Study 1\\Data used (working)\\3.csv", header = T, sep = ";")
data_202009 = read.table(file = "C:\\Users\\wicka\\Desktop\\Google Data Analytics certification\\Course 8 - Capstone project - Complete a case study\\Case Study 1\\Data used (working)\\4.csv", header = T, sep = ";")
data_202010 = read.table(file = "C:\\Users\\wicka\\Desktop\\Google Data Analytics certification\\Course 8 - Capstone project - Complete a case study\\Case Study 1\\Data used (working)\\5.csv", header = T, sep = ";")
data_202011 = read.table(file = "C:\\Users\\wicka\\Desktop\\Google Data Analytics certification\\Course 8 - Capstone project - Complete a case study\\Case Study 1\\Data used (working)\\6.csv", header = T, sep = ";")
data_202012 = read.table(file = "C:\\Users\\wicka\\Desktop\\Google Data Analytics certification\\Course 8 - Capstone project - Complete a case study\\Case Study 1\\Data used (working)\\7.csv", header = T, sep = ";")
data_202101 = read.table(file = "C:\\Users\\wicka\\Desktop\\Google Data Analytics certification\\Course 8 - Capstone project - Complete a case study\\Case Study 1\\Data used (working)\\8.csv", header = T, sep = ";")
data_202102 = read.table(file = "C:\\Users\\wicka\\Desktop\\Google Data Analytics certification\\Course 8 - Capstone project - Complete a case study\\Case Study 1\\Data used (working)\\9.csv", header = T, sep = ";")
data_202103 = read.table(file = "C:\\Users\\wicka\\Desktop\\Google Data Analytics certification\\Course 8 - Capstone project - Complete a case study\\Case Study 1\\Data used (working)\\10.csv", header = T, sep = ";")
data_202104 = read.table(file = "C:\\Users\\wicka\\Desktop\\Google Data Analytics certification\\Course 8 - Capstone project - Complete a case study\\Case Study 1\\Data used (working)\\11.csv", header = T, sep = ";")
data_202105 = read.table(file = "C:\\Users\\wicka\\Desktop\\Google Data Analytics certification\\Course 8 - Capstone project - Complete a case study\\Case Study 1\\Data used (working)\\12.csv", header = T, sep = ";")

wholeyeardata = bind_rows(data_202006,data_202007,data_202008,data_202009,data_202010,data_202011,data_202012,data_202101,data_202102,data_202103,data_202104,data_202105)

table(wholeyeardata$member_casual)
```

Using the last line of code, we find that the number of riders are:

casual = 1712446
member = 2357821
 

Another problem in the data is that some ride_length entries are 00:00:00, which is not logically possible. Thus I filtered those out, as they are likely due to customers hiring a bike by accident and then immediately cancelling. These entries might skew the data in an unwanted direction, and can thus be removed without negatively impacting our analysis.


<br/><br/>
### Step 5 - Visualisation and presentation ✨
<br/><br/>
### Step 6 - Call to action 💡

<br/><br/>

<a name="case2"></a>
## Case Study 2 - Guide a marketing strategy based on how users interact with fitness smart devices 

<p align="center">
  <img width="310p" src="https://github.com/nuclearcheesecake/wickusgoogledataanalyticscertificate2021/blob/main/Misc/andres-urena-V7UoMNWsYsg-unsplash.jpg">
</p>

(For the scenario supplied by Google, see [here](https://github.com/nuclearcheesecake/wickusgoogledataanalyticscertificate2021/blob/main/Case%20study%202/case2.pdf).)

### Step 1 - Initial scenario investigation 👔

* **The stakeholders and important players in this project**

* **What problem am I trying to solve?**

* **How can my insights drive business decisions?**

<br/><br/>

### Step 2 - Obtaining the correct data 📜

For this project, I will use data from June 2020 to May 2021, as this is the most recent data available at the time of analysis (July 2021). The data for this project is located in a [public data source](https://divvy-tripdata.s3.amazonaws.com/index.html). 

* **Storing and organising the data**


* **Bias and credibility**

Since data has been collected on both casual riders and members, it is not skewed towards one. We have data about the whole population - quite a unique situation! 

We can further use the ROCCC analysis as suggested by the course to see if the data is unbiased:

- Reliable ✔️ - We are using the company's own data
- Original ✔️ - Data used is internal, original copies
- Comprehensive ✔️ - Contains enough attributes on cyclist info to be useful
- Current ✔️ - We obtained data from the last 12 months
- Cited ✔️ - We are using the company's own data

Thus we can say that the data we have gathered is certain to be unbiased. The results obtained can thus be seen as credible.


* **Licensing, privacy, security and accessibility**

* **Verifying the data's integrity**

* **How will the data help me answer the proposed question?**

* **Problems found with the data**


<br/><br/>

### Step 3 - Cleaning and processing the data 🧹️

* **Dealing with missing data**

* **Checking for entry errors**

* **Removing duplicates**

* **Calculated rows**



<br/><br/>

### Step 4 - Analysis 🕵️‍♂️
<br/><br/>
### Step 5 - Visualisation and presentation ✨
<br/><br/>
### Step 6 - Call to action 💡

<br/><br/>

<a name="case3"></a>
## Case Study 3 - My own case study

## Conclusion

<p align="center">
  <img width="240p" src="https://github.com/nuclearcheesecake/wickusgoogledataanalyticscertificate2021/blob/main/Misc/badge.png">
</p>
