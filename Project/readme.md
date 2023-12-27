# Alcohol Tolerance Prediction
### INDENG 242 Final Project
### Xiaozhe Liu, Ziyang Wei, Zehua Qiu, Zekun Li, Zhiding Zhang

## Step 1: Collect data
We design a survey to collect data
- Purpose of the Survey:
This survey is designed to gather information on various factors that may influence an individual's alcohol tolerance. Our goal is to better understand how different elements such as health, lifestyle, and personal habits contribute to the amount of alcohol a person can consume before showing signs of intoxication.

- Confidentiality Assurance:
Responses will be kept strictly confidential. No personally identifiable information is collected, ensuring that your answers remain anonymous.

Variables:
- age, sex, weight(Kg), hight(cm), smoke(1-smoke, 2-no smoke)
- `drinking_freq`: Drinking Frequency, 1 = Daily; 2 = Weekly; 3 = Monthly; 4 = Yearly, 5 = Rarely
- `month_drinking_freq`: How many times do you typically consume alcoholic beverages in a month? (1,2, ...)
- `drinking_legth`: For each time you drink, how long you spend on it. 1 = 1-2hours; 2 = 2-3hours; 3 = 3-4hours; 4 = 4hours and more; 5 = do not drink
- `parent_freq`: How often your parent drink alcohol. 1 = Very often(At least one times a week); 2 = Often(About one times a week); 3 = Not often(About one time in several month); 4 = Barely(About 1 or 2 times in a year); 5 = Never
- `eating_2`: About 2 hour before drinking, do you eat? 1 = Always; 2 = Often; 3 = Sometimes; 4 = Never
- `stress_level`: Stress Level when you drinking. 1 = Feel very stress(or feels bad); 2 = Stress; 3 = not too stress in majority of times; 4 = not stress at all
- `sleep_length`: average sleep length in hours
- `liver_cond`: Do you have any known liver health conditions? This includes conditions such as hepatitis, cirrhosis, or other liver-related health issues. 1 = yes; 2 = no
- `tolerance`: On average, how many standard drinks do you believe you could consume before reaching a point of losing consciousness? (1,2,...)
- `workout_freq`: How often you go fitness(Cardio, Anaerobic or sports). 1 = Very often(At least 3 times a week), 2 = Often(About one times a week); 3 = Not often(About one time in several month); 4 = Barely(About 1 or 2 times in a year); 5 = Never

## Step 2, Clean The Data
Most of the data are good. But since we did not put many contrain in survey, some of the data are not in a good shape. For example, people type in unit(55KG), incorrect unit(1.70m instead 170), Chinese character, exaggerated numbers and irrelevant information for the free respond questions. So we clean the data by hand since we only collected about 500 datas. 

Also, we need to manual assign the datatype and change some of the multiple choice answers to categorie values(often, not often..)