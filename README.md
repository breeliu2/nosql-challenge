# nosql-challenge
In this challenge, we were instructed to evaluate some of the ratings from a food magazine, Eat Safe, Love, in order to help their journalists and food critics decide where to focus future articles. 

## Part 1: Database and Jupyter Notebook Set Up 
 NoSQL_setup_starter.ipynb was used for this section
 1. Imported the data with mongoimport --tyoe json -d uk_food -c establishments --drop --jsonArray establishments.json
 2. Import PyMongo and Pretty Print
 3. Create an instance of the Mongo Client
 4. Confirm that the database was created and loaded properly

## Part 2: Update the Database
Make the following changes to the establishments collection: 
1. Add the following info to the database: 
{
    "BusinessName":"Penang Flavours",
    "BusinessType":"Restaurant/Cafe/Canteen",
    "BusinessTypeID":"",
    "AddressLine1":"Penang Flavours",
    "AddressLine2":"146A Plumstead Rd",
    "AddressLine3":"London",
    "AddressLine4":"",
    "PostCode":"SE18 7DY",
    "Phone":"",
    "LocalAuthorityCode":"511",
    "LocalAuthorityName":"Greenwich",
    "LocalAuthorityWebSite":"http://www.royalgreenwich.gov.uk",
    "LocalAuthorityEmailAddress":"health@royalgreenwich.gov.uk",
    "scores":{
        "Hygiene":"",
        "Structural":"",
        "ConfidenceInManagement":""
    },
    "SchemeType":"FHRS",
    "geocode":{
        "longitude":"0.08384000",
        "latitude":"51.49014200"
    },
    "RightToReply":"",
    "Distance":4623.9723280747176,
    "NewRatingPending":True
}
2. Find the BusinessTypeId for "Restaurant/Cafe/Canteen" and return only BusinessTypeID and BusinessType fields.
3. Update the new restaurant with the BusinessTypeID
4. Remove any establishments within the Dover Local Authority and check to ensure they were deleted. 
5. Update latitude and longitude to decimal numbers and RatingValue to integer numbers.

## Exploratory Analysis
Answer the following questions from Eat, Safe, Love to help them find the locations they want to visit and avoid. 
1. Which establishments have a hygiene score equal to 20?
2. Which establishments in London have a RatingValue greater than or equal to 4?
3. What are the top 5 establishments with a RatingValue rating of 5, sorted by lowest hygiene score, nearest to the new restaurant added, "Penang Flavours"?
4. How many establishments in each Local Authority area have a hygiene score of 0?

