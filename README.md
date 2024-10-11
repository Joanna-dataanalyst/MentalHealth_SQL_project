# MentalHealth_SQL_project
Does going to university in a different country affect your mental health? A Japanese international university surveyed its students in 2018 and published a study the following year that was approved by several ethical and regulatory boards.

The study found that international students have a higher risk of mental health difficulties than the general population, and that social connectedness (belonging to a social group) and acculturative stress (stress associated with joining a new culture) are predictive of depression.

Explore the students data using PostgreSQL to find out if you would come to a similar conclusion for international students and see if the length of stay is a contributing factor.

Here is a data description of the columns you may find helpful.

<img width="374" alt="Screenshot 2024-10-11 103004" src="https://github.com/user-attachments/assets/557f0a17-0ce2-49cc-9af4-ae28cd45e81e">

### In [1]:
![image](https://github.com/user-attachments/assets/4600a9b7-ca75-468a-a548-18125ff08847)


### Out [1]:
![image](https://github.com/user-attachments/assets/e6164211-0b47-43df-9690-dc5b22ea958f)

### In [2]: -- Count the number of record in the dataset
![image](https://github.com/user-attachments/assets/d5b2bba7-20f8-4d02-9ea0-cba75fe46e6f)

### Out [2]:
![image](https://github.com/user-attachments/assets/ceb8a164-17a6-4410-9510-cd7fbbb63dec)

### In [3]: -- inspect dataset and limit the ouput to 5 records
![image](https://github.com/user-attachments/assets/1b5b445b-81c8-4f9a-9418-c207a2b56942)

### Out [3]: 
![image](https://github.com/user-attachments/assets/2eb9db3c-4892-45d1-9599-003ddc12f2fd)

### In [4]: -- how many international students and domestic students are in the dataset
![image](https://github.com/user-attachments/assets/3ba32c1b-9f10-418f-af4c-2d3349679fee)

### Out [4]: 
![image](https://github.com/user-attachments/assets/afea9e53-1925-497d-a0db-3c8e646eacd9)

### In [5]: -- fix the spelling error on the interdom column name
![image](https://github.com/user-attachments/assets/7feb413a-e7f9-47f3-9cf3-0eb942e8b23c)

### Out [5]: 
![image](https://github.com/user-attachments/assets/1b359464-e2e6-4690-8695-2316cb02d37b)

### In [6]: -- where are the international students from? see the regions where they come from
![image](https://github.com/user-attachments/assets/406d515e-b7a6-458f-ad05-4bbbb1964d5d)

### Out [6]: 
![image](https://github.com/user-attachments/assets/c1d8143c-04f4-4947-96a0-1740adb57b7f)

### In [7]: -- find the min, max, avg of the diagnostic tests(todep,phq-9)(tosc,scs)(toas,asiss)
![image](https://github.com/user-attachments/assets/abd54903-b616-4775-8a59-39c7117195d3)

### Out [7]: 
![image](https://github.com/user-attachments/assets/a4664b74-d794-4ce6-898a-cd1575f35cae)

### In [8]:-- what is the number of male and female students that took the test
![image](https://github.com/user-attachments/assets/58a30722-702b-4b8b-aa28-97ec0d9d5bbf)

### Out [8]: 
![image](https://github.com/user-attachments/assets/5b8aa80d-f242-4017-81b2-a3aa2d9f7c99)

### In [9]:-- what is the number of international female students
![image](https://github.com/user-attachments/assets/d380d21a-fc0b-43fa-b28e-075abba3e4d4)

### Out [9]: 
![image](https://github.com/user-attachments/assets/d507a764-11a1-4eac-9bc9-19e0e73767b9)

### In [10]: -- what is the number of grads and undergrads that took the test
![image](https://github.com/user-attachments/assets/30e952d8-bba7-46ad-9eef-82ce352db955)

### Out [10]: 
![image](https://github.com/user-attachments/assets/ef1a8bd3-e21c-41c2-b20b-ee328b11b148)

### In [11]:-- how many male and female students greater > than the age of 30 took the test
![image](https://github.com/user-attachments/assets/52eca59a-c0ee-434d-82c8-c2f50a5d2fdc)

### Out [11]: 
![image](https://github.com/user-attachments/assets/dea00f94-ad64-41cf-858d-a6e3bfdb27b6)

### In [12]:-- how many male and female students less < than or = the age of 20 took the test
![image](https://github.com/user-attachments/assets/e9910ca5-e11f-4fe9-9666-5568b714d3ee)

### Out [12]: 
![image](https://github.com/user-attachments/assets/1f939ccc-67b3-4833-a4bd-59c04a301004)







