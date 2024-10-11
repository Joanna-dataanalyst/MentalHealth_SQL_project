# SQL-Employee-Analytics
Does going to university in a different country affect your mental health? A Japanese international university surveyed its students in 2018 and published a study the following year that was approved by several ethical and regulatory boards.

The study found that international students have a higher risk of mental health difficulties than the general population, and that social connectedness (belonging to a social group) and acculturative stress (stress associated with joining a new culture) are predictive of depression.

Explore the students data using PostgreSQL to find out if you would come to a similar conclusion for international students and see if the length of stay is a contributing factor.

Here is a data description of the columns you may find helpful.

<img width="374" alt="Screenshot 2024-10-11 103004" src="https://github.com/user-attachments/assets/557f0a17-0ce2-49cc-9af4-ae28cd45e81e">

# In [1]: select * from `mental health analysis`;

# Out [1]:

![image](https://github.com/user-attachments/assets/e6164211-0b47-43df-9690-dc5b22ea958f)

# In [2]: -- Count the number of record in the dataset
SELECT count(*) AS totalRecord
FROM `mental health analysis` ;

# Out [2]:

![image](https://github.com/user-attachments/assets/ceb8a164-17a6-4410-9510-cd7fbbb63dec)


# In [3]: -- inspect dataset and limit the ouput to 5 records
Select *
from `mental health analysis`
limit 5;

# Out [3]: 

![image](https://github.com/user-attachments/assets/2eb9db3c-4892-45d1-9599-003ddc12f2fd)

# In [4]: -- how many international students and domestic students are in the dataset
select ï»¿inter_dom, 
count(ï»¿inter_dom) as count_inter_dom
from `mental health analysis`
group by ï»¿inter_dom;

# Out [4]: 

![image](https://github.com/user-attachments/assets/afea9e53-1925-497d-a0db-3c8e646eacd9)













