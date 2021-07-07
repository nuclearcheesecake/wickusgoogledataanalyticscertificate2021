# My capstone case studies for the Google Data Analytics Certificate

During some free time at university, I enrolled in the [Google Data Analytics Professional Certificate on Coursera](https://www.coursera.org/professional-certificates/google-data-analytics?utm_source=gg&utm_medium=sem&utm_campaign=15-GoogleDataAnalytics-ROW&utm_content=15-GoogleDataAnalytics-ROW&campaignid=12566515400&adgroupid=117869292845&device=c&keyword=google%20data%20certification&matchtype=b&network=g&devicemodel=&adpostion=&creativeid=507290840621&hide_mobile_promo&gclid=CjwKCAjwieuGBhAsEiwA1Ly_nW0b8kYk9covlwaMOn7AAHj-pwimBJu1BJoDXrcxvuykE_Vm3paHGRoCdfYQAvD_BwE) to sharpen my skills with data analytics tools that I want to use. In the process, I was greeted by a collection of instructors that each handed me the start of a thread that lead deeper into the tapestry of analytics. 

<p align="center">
  <img width="825" src="https://github.com/nuclearcheesecake/wickusgoogledataanalyticscertificate2021/blob/main/Misc/course.png">
</p>

This is due to the course having a strong focus on the methodology of data analytics projects, with each phase representing an area of expertise to explore. The phases that Google suggests are:

* Ask, or a preliminary analysis of the scenario (stakeholder and problem analyses)
* Prepare, or collecting and storing data for our specific analysis
* Process, or cleaning and preparing the data for analysis
* Analyse, or finding patterns and generating insights using the data
* Share, or creating visualisations and presentations
* Act, or taking action with stakeholders given the new insights

To complete the certificate, I had to design and complete a case study that implements this methodology, as was taught in the course. I had three options for the case study, but, in the interest of gaining more practice with my data analytics tools, I decided that all three are good applications to explore. Thus in this repositiory, you will find the following three case studies that I have completed using the methodology above:

1. [Developing a new marketing strategy to increase influx of annual memberships at a bike-sharing company (with a focus on **Microsoft Excel**)](#case1)
2. [Guide a marketing strategy based on how users interact with fitness smart devices (with a focus on **SQL**)](#case2)
3. [Case study 3 (with a focus on **R**)](#case3)

The first two are theoretical case studies created by Google, and thus all the data was provided by them. For the last option, however, I had to find an alternative data source. Here follows my three case studies. As stated above, these case studies will implement the Google Data Analytics methodology. To further test out my toolset, I decided to attempt all 3 case studies with a primary focus on a singular tool (stated boldly in brackets above).

<a name="case1"></a>
## Case Study 1 - Developing a new marketing strategy to increase influx of annual memberships at a bike-sharing company

<p align="center">
  <img width="310p" src="https://github.com/nuclearcheesecake/wickusgoogledataanalyticscertificate2021/blob/main/Misc/carl-nenzen-loven-igKjieyjcko-unsplash.jpg">
</p>

(For the scenario supplied by Google, see [here](https://github.com/nuclearcheesecake/wickusgoogledataanalyticscertificate2021/blob/main/Case%20study%201/case1.pdf).)

### Step 1 - Initial scenario investigation

In this scenario, I am a junior data analyst working for the marketing analyst team at **Cyclistic**, a company in Chicago with a bike-sharing program that is important to its operation. This team now has the goal of guiding the future marketing program, and I was tasked with a specific question to answer:

*How do annual members and casual rides use Cylistic bikes differently?*

At the end of my analysis, I am expected to hand in a report summarising all the steps I took, and my recommendations for a marketing campaign. I will be using this space on GitHub to jot down my thoughts in the process of answering this question - but if you are interested only in the final deliverable, click HERE.


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


### Step 2 - Obtaining the correct data

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


* **Licensing, privacy, security and accessibility**


* **Verifying the data's integrity**


* **How will the data help me answer the proposed question?**


* **Problems found with the data**




### Step 3 - Cleaning and processing the data

### Step 4 - Analysis

### Step 5 - Visualisation and presentation

### Step 6 - Call to action

<a name="case2"></a>
## Case Study - Guide a marketing strategy based on how users interact with fitness smart devices

<a name="case3"></a>
## Case Study 3 - My own case study

## Conclusion

<p align="center">
  <img width="240p" src="https://github.com/nuclearcheesecake/wickusgoogledataanalyticscertificate2021/blob/main/Misc/badge.png">
</p>
