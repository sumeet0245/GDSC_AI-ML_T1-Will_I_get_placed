## GDSC_AI-ML_T1-Will_I_get_placed
Beginner ML project to predict student placement using Logistic Regression as a beginner task for GDSC club inductions

## What is this project?
This is a machine learning project that predicts whether a student will get placed or not based on their academic performance, internships, and other factors.

## Dataset
The dataset has 10,000 students with information like:
- CGPA
- Number of internships done
- Projects completed
- Aptitude test score
- Soft skills rating
- Whether they did placement training
- Their final placement status (Placed or Not Placed)

## What I did

### 1. Data Analysis (EDA)
First, I analyzed the data to understand patterns:
- How many students got placed vs not placed
- What was the average CGPA of placed students
- Did students with more internships get placed more?
- How important is aptitude score for placement?

I made some graphs to visualize these patterns.

### 2. Preparing the Data
Before feeding data to the model, I had to:
- Convert text values (like "Yes", "No") into numbers (0, 1) so the model understands
- Scale all numbers to similar ranges (because CGPA is 0-10 but aptitude score is 0-100)
- Split data into 80% for training and 20% for testing

### 3. Building the Model
I used **Logistic Regression** (a basic ML algorithm that predicts if something happens or not).

The model learns from 8,000 students and tries to predict placement for 2,000 new students it hasn't seen before.

### 4. Testing the Model
I checked how well the model works:
- **Accuracy:** How many predictions were correct
- **Precision:** Of students the model said would be placed, how many actually got placed
- **Recall:** Of students who actually got placed, how many did the model find

The model got **more than 60% accuracy** which was the requirement.

## Files in this project
- `GDSC_T1.py` - The main code that runs everything
- `DATASET` - The student data

## How to run this

1. Install the required libraries:


2. Make sure the CSV file is in the same folder as the Python script

3. Run the script:
```bash
python placement_prediction.py
```

4. The script will:
   - Show data analysis and graphs
   - Train the model
   - Print accuracy and other scores
   - Make predictions on some sample students

## What I found out

1. **CGPA matters a lot** - Students with higher CGPA got placed more often
2. **Internships help** - Students who did 2 or more internships had better placement chances
3. **Aptitude score is important** - Students with higher aptitude scores got placed more
4. **Soft skills matter too** - Though less important than the above factors

## Model Performance

The model achieved good accuracy and can predict placement status with reasonable confidence.

## Challenges I faced

-understand the working of Lofistics Regression algorithms and where to use it
- Had to figure out how to handle text data (converting Yes/No to numbers)
- Understanding why we need to scale features (StandardScaler)
- Making sure the model doesn't overfit to training data

## Conclusion

This project shows how machine learning can be used to predict real-world outcomes like student placement. While the model works well, in real scenarios we would need more data and try other algorithms too.

## Author
ch.sumeet preetham

## Date
January 2026
