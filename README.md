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

To collect the data I utilized "Data.World", where users can discover data, share analysis and team up all over the world. Using "Datafiniti's Product database" I was able to locate an extensive list of product data. 

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

FIRST I STARTED BY LOADING THE TWO TABLES INTO THE `PortfolioProject` DATABASE IN MYSQL. BELOW I AM SHOWING HOW THE TABLE LOOKS BEFORE ANY ANALYSIS
IS COMPLETED. 

Mens Shoes Table Before Any Cleaning Implemented: 


<img width="1440" alt="Screen Shot 2022-10-22 at 10 07 22 PM 1" src="https://user-images.githubusercontent.com/109754836/197371444-76be8b36-8bdc-455c-b5d3-4e4abbe10cb6.png">

WOMENS SHOES TABLE BEFORE ANY CLEANING IMPLEMENTED:

<img width="1440" alt="Screen Shot 2022-10-22 at 10 16 22 PM" src="https://user-images.githubusercontent.com/109754836/197371658-2e0f33a8-a921-47d1-9ee9-b1a4d9b75603.png">

     ------ NEXT I TOOK A FIRST GLANCE AT BOTH TABLES. GETTING A BETTER SENSE OF WHAT THE TABLES ARE ABOUT, 
     WHAT THEY INCLUDE, ETC. TO PREPARE FOR DATA CLEANSING -------
     
<img width="1440" alt="Screen Shot 2022-10-22 at 10 22 23 PM" src="https://user-images.githubusercontent.com/109754836/197371838-21536131-b2c8-44f2-a1ee-952d63b5475f.png">

      ------ ALREADY I AM NOTICING BOTH TABLES NEED EXTENSIVE CLEANING, THEREFORE I AM REFFERING BACK TO THE 
      BUSINESS OBSTACLE I AM TRYING TO SOLVE WITH THIS DATA. EVERY DATASET IS DIFFERENT, FURTHERMORE REFERRING 
      BACK TO THE BUSINESS OBSTACLE, WILL ALLOW ME TO UNDERSTAND WHAT I NEED TO KEEP AND WHAT DATA CAN BE EXCLUDED. ----
      
So starting with the `mens shoes` table I used Excel to clean up the columns, fix the column names, delete the columns I dont need, and delete duplicate 
Columns. 

- I will need to do the same for `womens shoes`table here...

<img width="1440" alt="Screen Shot 2022-10-22 at 10 44 05 PM" src="https://user-images.githubusercontent.com/109754836/197372584-3c0f1959-a091-4c4f-8eab-e57d5b29a5e7.png">







