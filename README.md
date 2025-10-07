**CAPSTONE PROJECT
HEALTHCARE DATASET ANALYSIS**

~~~sql
-- Phân phối theo nhóm tuổi
SELECT age_group, COUNT(*) AS patients,
        ROUND(100.0 * COUNT(*) / SUM(COUNT(*)) OVER(), 2) AS pct_of_total
FROM v_healthcare_analysis
GROUP BY  age_group
ORDER BY patients DESC;


-- Phân phối theo giới tính
SELECT gender, COUNT(*) AS patients,
ROUND(100.0 * COUNT(*) / SUM(COUNT(*)) OVER(),2) AS pct_of_total
FROM v_healthcare_analysis
GROUP BY gender
ORDER BY patients DESC;

-- Phân phối theo nhóm máu
SELECT blood_type, COUNT(*) AS patients, 
       ROUND(100.0 * COUNT(*) / SUM(COUNT(*)) OVER(),2) AS pct_of_total
FROM v_healthcare_analysis
GROUP BY blood_type
ORDER BY patients DESC;
~~~

|blood_type|patients|pct_of_total|
|---|---|---|
|A+|19425|35.0000000000000|
|O+|13875|25.0000000000000|
|O-|8325|15.0000000000000|
|AB-|2775|5.0000000000000|
|B+|2775|5.0000000000000|
|A-|2775|5.0000000000000|
|AB+|2775|5.0000000000000|
|B-|2775|5.0000000000000|
