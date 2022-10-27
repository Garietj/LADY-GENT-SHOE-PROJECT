# LADY & GENT SHOE PROJECT(DATA CLEANSING P1)
BY JASMINE GARIET AKA JAZZYANALYTICS

MEN AND WOMEN SHOE PORTFOLIO PROJECT FOCUSED ON GAINING INSIGHTS INTO THE CORRELATION BETWEEN MEN AND WOMENS SHOE PRODUCTS, AND MORE.

# INTRODUCTION: 
    This portfolio project series consists of a thorough business walk through implementing a variation
    of data-based analytical tools.
    Visualizations, Insights, Summaries, and Conclusions will be presented in a comprehensive construct. 
    Revealing every organized step that was utilized to introduce the audience to my Data Analysis mindset
    and problem solving capabilities. As a freelance Fashion Designer as well as a huge hobby of mine,
    I absolutely love everything fashion. Shoes, Clothes, Accessories the list goes on. It was my mission to
    find a data set that correlated to my interest and passions. 
    
1.) ABOUT THE DATA
    
This is a list of 10,000 men's shoes provided by Datafiniti's Product Database.
The dataset includes shoe name, brand, price, and more. Each shoe will have an entry for each price found for it and some 
shoes may have multiple entries. 


This is a list of 10,000 women's shoes and their product information provided by Datafiniti's Product Database.
The dataset includes shoe name, brand, price, and more. Each shoe will have an entry for each price found for 
it and some shoes may have multiple entries.

    To collect the data I utilized "Data.World", where users can discover data, share analysis and team up 
    all over the world. Using "Datafiniti's Product database" I was able to locate an extensive list of product data. 

2.) BUSINESS OBSTACLE 
  
  I will Analyze Product Data for Men and Women's FootWear from some of the broadest known Brands like, "Kenneth Cole", "Stacy Adams", "Adidas", "Nike", "New Balance", "PUMA", "Steve Madden" and many more. The primary objective for this project is to gain insights into the correlation between the men and women Footwear using data driven resolutions to answer the following business task below: 


- What are the diffences between Men and Womens shoe prices?
- Which brands have the highest prices?
- What is the average price of each distinct brand listed?
- Correlate specific product features with changes in price.
-  Cross reference the data with mens and womens shoe prices to see if there are any differences between women's brands and men's brands.

I will split this project into 3 segments:
1.) Data Cleansing 
2.) Data Exploration 
3.) Data Visualization 

# -- LADY & GENT SHOE PROJECT (DATA CLEANSING SEGMENT)--

FIRST I STARTED BY LOADING THE TWO TABLES INTO THE `PortfolioProject` DATABASE IN MYSQL. BELOW I AM SHOWING HOW THE TABLES LOOK IN EXCEL
BEFORE ANY ANALYSIS IS COMPLETED. 

MENS SHOES TABLE BEFORE ANY CLEANING IMPLEMENTED: 


<img width="1440" alt="Screen Shot 2022-10-22 at 10 07 22 PM 1" src="https://user-images.githubusercontent.com/109754836/197371444-76be8b36-8bdc-455c-b5d3-4e4abbe10cb6.png">

WOMENS SHOES TABLE BEFORE ANY CLEANING IMPLEMENTED:

<img width="1440" alt="Screen Shot 2022-10-22 at 10 16 22 PM" src="https://user-images.githubusercontent.com/109754836/197371658-2e0f33a8-a921-47d1-9ee9-b1a4d9b75603.png">

     ------ NEXT I TOOK A FIRST GLANCE AT BOTH TABLES. GETTING A BETTER SENSE OF WHAT THE TABLES ARE ABOUT, 
     WHAT THEY INCLUDE, ETC. TO PREPARE FOR DATA CLEANSING -------
     
<img width="1440" alt="Screen Shot 2022-10-22 at 10 22 23 PM" src="https://user-images.githubusercontent.com/109754836/197371838-21536131-b2c8-44f2-a1ee-952d63b5475f.png">

      ------ ALREADY I NOTICED BOTH TABLES NEEDED EXTENSIVE CLEANING, THEREFORE I REFFERED BACK TO THE 
      BUSINESS OBSTACLE I AM TRYING TO SOLVE WITH THIS DATA. EVERY DATASET IS DIFFERENT, FURTHERMORE REFERRING 
      BACK TO THE BUSINESS OBSTACLE, WILL ALLOW ME TO UNDERSTAND WHAT I NEED TO KEEP AND WHAT DATA CAN BE EXCLUDED. ----
      
So starting with the `mens shoes` table I used Excel to clean up the columns, fix the column names, delete the columns I dont need, and delete duplicate 
Columns. 

- I proceeded to implement the same for the `womens shoes`table using MySQL...

<img width="1440" alt="Screen Shot 2022-10-22 at 10 44 05 PM" src="https://user-images.githubusercontent.com/109754836/197372584-3c0f1959-a091-4c4f-8eab-e57d5b29a5e7.png">

<img width="769" alt="Screen Shot 2022-10-26 at 4 47 11 PM" src="https://user-images.githubusercontent.com/109754836/198145003-f4fcf687-99bf-4f0f-956b-bb5dc68f78eb.png">

<img width="568" alt="Screen Shot 2022-10-26 at 4 50 01 PM" src="https://user-images.githubusercontent.com/109754836/198145402-035cfbfc-0838-4c41-ab17-c2e1a59b7d57.png">

- Now, I dropped all the columns I did not need in the `Womens Shoes` Table and also dropped a few 
more columns from the mens table.
- Next I went ahead and Fixed the column names by renaming them and capitalizing the first letter, making the column names visually appealing. 

I started with the `Womens Shoes` Table : Since I already started editing the mens table in Excel there was not much to do. 

<img width="683" alt="Screen Shot 2022-10-26 at 5 11 13 PM" src="https://user-images.githubusercontent.com/109754836/198148379-e49e63d6-cd6d-4a82-ace2-31990bca4535.png">

- Upon looking at the data in the table I noticed while fixing the column names in the `mens shoes` table that the 'Date Seen' 
information and 'Date Added' columns should be switched. All that needed to be done was to switch the column names. showing below:

<img width="1299" alt="Screen Shot 2022-10-26 at 5 17 06 PM" src="https://user-images.githubusercontent.com/109754836/198149154-90a2a7e0-e690-40dd-b81c-1128750a3859.png">

- IN EXCEL I CONVERTED THE `MENS SHOES` DATEtime COLUMN IN EXCEL, SO I WENT AHEAD AND CONVERTED THE `WOMENS SHOES` DATEtime COLUMN IN MYSQL:

<img width="749" alt="Screen Shot 2022-10-26 at 5 21 53 PM" src="https://user-images.githubusercontent.com/109754836/198151102-75c9c541-47be-4cd4-8c00-287edc54e13f.png">

     * NOTICE ON THE LAST SQL SYNTAX THE RED ERROR BAR. THE SYNTAX IS CORRECT AND NO ERROR CODE WAS GENERATED IN 
     THE RESULTS GRID, YET IT IS SHOWING A RED LINE ON THE BOTTOM. FURTHER RESEARCH SUGGEST THAT IT HAPPENS WHEN THE 
     USER HAS A SPECIFIC VERSION OF MYSQL. IT'S A BUG THAT IS SUPPOSED TO BE FIXED WITH MY VERSION 8.0.30
     THE NEWEST VERSION. SQL CODE IS POSTED IN THE LADY-GENT-SHOE PROJECT REPOSITORY. *
     
     
 - After converting the datetime in the `Womens Shoes` table I noticed a few more columns that needed to be switched/renamed and went ahead and changed that.
 - Once I went through the `Womens Shoes` table I noticed there was a 'Brand Name' named 'SALE'. Realizing that this could be a possible outlier, I ran the following query below and received 4 results back that include brand name as 'SALE'.

<img width="1162" alt="Screen Shot 2022-10-26 at 6 00 27 PM" src="https://user-images.githubusercontent.com/109754836/198154655-dd58ff04-26c2-4be9-b2ea-4e51c7598cea.png">

<img width="1439" alt="Screen Shot 2022-10-26 at 6 07 28 PM" src="https://user-images.githubusercontent.com/109754836/198155695-e76ab043-445a-4347-867e-fd5c64fe3085.png">

- After further research I noticed the Sale brand was added on the same day, time, date seen, they have different IDs and different shoe sizes. Which let's me know that they are a variety of shoes within that brand and in fact meant to be in the table and not a mistake. I decided to leave the 'Sale' Brand name as is, not wanting to interfere with the data. There was not enough evidence to suggest it was an invalid Brand name input. 

        I then went through the data in both tables checking to see if there is anything else needed to clean...
        
<img width="632" alt="Screen Shot 2022-10-26 at 9 28 17 PM" src="https://user-images.githubusercontent.com/109754836/198176794-17c963b4-2a34-477b-bc3b-0385a8fda9a5.png">

- So these tables specifically the `Mens Shoes` table had a ton of missing values in the 'Colors', 'Brand names', and 'Sizes' columns. Instead of keeping them blank I needed to do further research to find the missing values. Further research into the table showed that most of the information I needed was in the 'SourceUrls' column which shows the description of the footwear, colors, distributors, sizes, and brand names. I went through each missing value; compared and contrasted the information I needed out and filled the missing values in. 
- There were other values like the variations of colors and sizes that were not able to be found in the 'SourceUrls' column. The strategy I took to overcome this was copying and pasting the Shoes ID, or the SourceURL, heading to "Google" and pasting the ID into the search handle. I really had to be strategic and really implement my researching skills to be able to locate all the missing values for this data. Luckily, I was able to find most of the missing information. "Google" located a ton of the shoes by ID or description of the shoe, So I was able to fill in all the missing values successfully. 
     For Example:
     <img width="808" alt="Screen Shot 2022-10-26 at 10 25 22 PM" src="https://user-images.githubusercontent.com/109754836/198184108-6bd270f3-aa2c-41a1-8f22-8af62a4b120c.png">



















