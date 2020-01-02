# Midterm2
Clone this for Midterm 2 - Nov 11, 2019

Clone this repository and then create your own brach from the main to work on it.
One done- push it to your main branch and put in a pull request- indicating you have submitted your exam.
The exam are back due next Monday  November 18, 2019 at 9:00 AM.

PARTs 1-2 and 3 are required, PART 4 is bonus.
Also - find attached extra credit questions from Brendan in the PDF file(exam2_extra.pdf).
You can submit answers to the questions in the PDF with a knitted markdown file, pushed into your branch with the rest of your exam.


Do not push to the main!!

The tasks are listed in the R script in the project file- use it as a template for your own work!
Here is a summary of the questions for a sneak peak.

# PART 1 ## Environmental Effects Evaluation
# Submit a visual and output for each question below

 1.Is location effect significant?
 a. What fraction of the variation observed in yield is attributable to
     Location specific effects?
 b. Which location seems to be the highest yield location?

 2. Is Company effect significant?
 a.Which company's varieties seem to perform the best across all regions?
 b.Which company's varieties seem to perform the worst across all regions?

 3. Is Region effect significant? How much variation in yield does region explain alone?
 How about together with Company?
 c.Which company's varieties seem to perform the best within each region?
 d.Which company's varieties seem to perform the worst within  each region?

 4. Is location effect significant together with Company and Region?
 e.Which company's varieties seem to perform the best for each location?
 f.Which company's varieties seem to perform the worst for each location?

 5. Does the seed treatments have a significant effect on the yield?
 a.Which treatment seems to have the largest positive effect? Is it significant?
 b.What fraction of the variation observed in yield is attributable to seed treatments?

 6. What is the best model for explaining the variation in the yield data,WITHOUT GENOS!
 Which location should I choose to use with which company's product
 to get the maximum yield? Should I apply Seed Treatment or not?

 7. Give your best prediction of maximum yield under these best case scenario conditions.
 Which location should I choose to use with which company's product
 to get the maximum yield? Should I apply Seed Treatment or not?
 Give your best prediction of maximum yield under these best case scenario conditions.


# PART 2 ## Genetic Effects Evaluation
# Submit a visual and output for each question below

 The variables qmx1..qmx369  each represent a "genetic_marker" that was scored on
 the entries that were included in the trials to identify if there are any genetic
 determinants that can be identified for high-yield.
 There are a total of 369 factor variables- with 2 states each {0,1} that are scored
 NOTE THAT YOU CAN NOT USE VARIETY AND GENOTYPE at the SAME TIME
 GENOTYPE marker data Defines VARIETY!!

 Using the example code for LASSO regression provided - fit a LASSO model
 to the data and investigate these marker variables for potential significant positive effects.
 Give your best prediction of maximum yield for a hypothetical variety, under the best
 possible environmental conditions we can offer.

 1. Does the model fit improve with marker data?
 2. Generate a list of markers that seem to have significant positive effects on yield,
 and provide their coefficients.

 Which location should I choose to use with which company's product
 to get the maximum yield? Should I apply Seed Treatment or not?
 Give your best prediction of maximum yield under these best case scenario conditions.


# PART 3 ## Visualization
# Submit a visual and output for each question below

 1. Yield Distributions by location 
 a. Density Plot
 b. box whisker plot by location
 c. density plot by Company
 d. box whisker plot by Company ordered by median yield for company
 e. box whisker plot by Company ordered by median yield for company, for each location

# PART 4 # BONUS # LOGISTIC  LASSO  REGRESSION ###
 Create a new binary variable based on the "Company" variable,
 where Companies whose products score at the top 5 performers across regions are coded as 1
 and the rest of the companies are coded as 0.
 Evaluate this variable versus the marker data [qmx1..qmx369] with ridge regression.
 Return the list of markers and their LASSO predicted coefficients from the model.
