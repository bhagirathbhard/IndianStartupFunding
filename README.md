## **<span style="color:#023e8a;font-size:200%"><center>Indian Startup Funding</center></span>**
## **<center><span style="color:#FEF1FE;background-color:#023e8a;border-radius: 5px;padding: 5px">By: Yicheng Jiang, Bhagirath Bhardwaj, Agnes Shih, Paul Seiters, and Siddharth Bookinkere</span></center>**

### **<span id="EDA" style="color:#023e8a;">Project and Dataset Overview</span>**

We are an old and very traditional money manager from the USA, investing almost exclusively in the US. After the US economy had lost a lot of its growth trajectory and the FED predicted GDP growth to linger below a mere 2% annually, our clients have been running from our investment products. Where are they all going? After booking a tee time with one of our long-time clients, we heard some adolescents with smartphones talking about the start-up scene in India. There were wild tales about startups with valuations beyond $1B, called unicorns. Apparently, there was not a hint of a slowing economy over there. Is it time to go international? After multiple people confirmed the start-up hype in India, we concluded that it is time to get ourselves a snapshot of what is going on in India. Who is investing? Where are they investing? And most importantly, which companies are they investing in? As a team, we perform data cleaning, exploratory data analysis, and finally, create a visualization in Tableau. Also, we chose the Indian Startup Funding dataset collected from multiple sources because of the varied types of funding covered, the sizable number of observations, and the time coverage from 2015 until May 2022, including the Covid-19 phase.

1.   Indian Startup Funding & Investment Chart [2021] (Trak.in link)
2.   Indian Startups - Funding & Investors Data [2018-2021] (Kaggle link)
3.   Indian Startup Funding & Investment Chart [2021] (Trak.in link)
4.   Indian Startups - Funding Data [2022] (Kaggle link)
5.   Funding details of the startups in India (Kaggle link)
6.   Cleaned Dataset from Github only for Funding calculation purpose and Dates - https://github.com/Satyampd/Startups-in-India-EDA/blob/master/dataset.csv

**In this project 2 datasets created for different purposes; Raw data from Kaggle in India_Funding data cleaning, union, etc.. Funding_Calculation created base on Github data source, for EDA analysis (AVG,SUBSTRING based on Funding, etc..)**

| Column      | Brief Description | Characteristic, Data type   |
| ----------- | ----------------  | ----------- |
| `UUID`      |  Randomly generated using `GENERATE_UUID()` bigquery function      |  String, Unique, Primary Key           |
| `Investors`   | Investor Name, usually an individual or a firm            |  String, multiple-values |
| `Funding_Year` | Year the start up was funded | Date |
| `Company_Brand` | Name of the startup | String, Not null |
| `Headquarter` | Location in City, Province where the startup was founded | String |
| `Stage` | Funding Round stage of the Startup, further described below* | String |
| `What_it_does` | Brief description about start-up | String |
| `USD_Amount` | Amount in USD funded per investment round | String |
| `Total_USD_Amount` | Calculated based on USD_Amount data | Integer (Data from github) |

**What is an investment stage?**
 
*   Many companies have to complete a number of fundraising rounds before getting to the initial public offering (IPO) stage.
*   These fundraising rounds allow investors to invest money into a growing company in exchange for equity/ownership.
*   The initial investment—also known as seed funding—is followed by various rounds, known as **Series A, B, and C**.
*  A new valuation is done at the time of each funding round.
Valuations are determined by various factors, including market size, company potential, current revenues, and management.

**ERD Diagram**

<img width="458" alt="download" src="https://user-images.githubusercontent.com/13074725/194221825-bfef8e2d-3c40-4924-971a-b50c78c39000.png">

