# Google PlayStore Analysis using PySpark

Agenda:
We have google playstore dataset ccontaining information of different apps, installed, rating, versions and other details and I did the analysis based on the data .

1. Find out TOP 10 reviews given to the apps.
2. Top 10 installs apps and distribution of type(free/paid)
3. Categorywise distribution of installed apps
4. Top paid apps
5. Top paid rating apps




### Steps followed 

- Step 1 : Install pyspark in Jupyter notebook
           !pip install pyspark
- Step 2 : Import libraries 
![Image](https://github.com/user-attachments/assets/a367e5cb-eae4-4b28-bc53-6fbc7bd53380)

    
- Step 3 :Load Files.
![Image](https://github.com/user-attachments/assets/595996b4-447b-4326-bb59-0316678d489b)


- Step 4 : Create a dataframe.
![Image](https://github.com/user-attachments/assets/b94f28f3-fc0f-4c10-bd28-56f56fd509e4)


- Step 5 : Check schema to mind any missing values, null values, data type mismatch and remove unneccessary columns.
![Image](https://github.com/user-attachments/assets/2924c031-9b14-457c-a139-95a1277e0d3c)


Found data type mismatch for "Reviews","Installs","Price","Rating"
- Step6 : Check Count
![Image](https://github.com/user-attachments/assets/80ce33f7-ddec-467e-9976-906663768ae2)


- Step7 : Data Cleaning performed.
- Step 7(a) : Removed "size","Content Rating","Last Updated","Android Ver","Current Ver".
![Image](https://github.com/user-attachments/assets/b44fd612-bb95-4218-8424-4e1f04b807e2)


- Step 7(b) :Changed data type of "Reviews","Installs","Price" to integer type and "Rating" to float type

- Step 7(c) : In "Installs" , there was "+" symbol, replaced it with "".
- Step 7(d) : In "Price" column, there was "$" ,it is replaced by "".
- Step 7(e) : In "Ratings" column, there was "NaN" ,it is replaced by "0".

![Image](https://github.com/user-attachments/assets/851596c5-46af-41de-9971-73ab9b6752e1)

![Image](https://github.com/user-attachments/assets/d1a4e0ce-46c0-4344-9f4e-eeac98ae5b57)

- Step 8 : Create a temporary view of the schema.
![Image](https://github.com/user-attachments/assets/ae84807e-c71a-43b6-b104-47b113484e63)


- Step 9 : First Query:Find out TOP 10 reviews given to the apps.
![Image](https://github.com/user-attachments/assets/57fa37ed-abfe-4ae7-8325-81c7f8356f15)


- Step 10 : Top 10 installs apps and distribution of type(free/paid). 
![Image](https://github.com/user-attachments/assets/3bdbdfe2-a352-4dd4-b15b-a190c45e3ffb)


- Step 11 : Categorywise distribution of installed apps. 
![Image](https://github.com/user-attachments/assets/4cbf2255-14f4-41a1-a9d0-bb28067fefcd)


- Step 12 : Top paid apps.
![Image](https://github.com/user-attachments/assets/39fec30e-5f29-4c26-ae24-467d1021731f)


- Step 13 : Top paid rating apps.
  ![Image](https://github.com/user-attachments/assets/774c4bab-9870-4ddd-bc07-cc92284c9378)
    
 

 
