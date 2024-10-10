# SQL-Employee-Analytics
create database Mental_health_analysis;
use Mental_health_analysis;

select * from smha;

-- count the number of records in the table
select count(*) as total_records from smha
;
 
 -- inspect dataset and limit the ouput to 5  records
Select *
from smha
limit 5;

-- how many international students and domestic students are in the dataset
select inter_dom, 
count(inter_dom) as count_inter_dom
from smha
group by inter_dom;

-- look into rows where data is null
select * from smha
where inter_dom not like 'D%' and 'i%' 
;

-- where are the international students from? see the regions where they come from
select region,count(inter_dom) as inter_region
from smha
where inter_dom = 'inter'
group by Region;

-- find the min, max, avg of the diagnostic tests(todep,phq-9)(tosc,scs)(toas,asiss)
select inter_dom,
       min(todep) as min_phq,
       max(Todep) as max_phq,
       avg(Todep) as avg_phq,
	
       min(ToSc) as min_scs,
       max(Tosc) as max_scs,
       avg(Tosc) as avg_scs,
       
		min(Toas) as min_asiss,
       max(Toas) as max_asiss,
       avg(Toas) as avg_asiss
       from smha
       where inter_dom in ('inter','dom')
       group by inter_dom;

-- what is the number of male and female students that took the test
select gender,count(gender) as count_gender
from smha
group by gender;

-- what is the number of international female students
select gender,count(inter_dom) as count_inter_dom_gender
from smha
where inter_dom = 'inter'
and gender = 'female'
group by gender
;

-- what is the number of grads and undergrads that took the test
select academic, count(academic) as count_academic
from smha
group by Academic;

-- how many male and female students greater than the age of 30 took the test
select gender, count(age) as count_age_gender
from smha
where age > 30
group by gender;

-- how many male and female students less than or = the age of 20 took the test
select gender, count(age) as count_age_gender
from smha
where age <= 20
group by gender;
