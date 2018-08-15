# Session-6.2-assignment-rahul-sharma
Acagild session 6.2 assignment

1. Import the Titanic Dataset from the link Titanic Data Set.

Perform the following:

a. Is there any difference in fares by different class of tickets?

Note - Show a boxplot displaying the distribution of fares by class

b. Is there any association with Passenger class and gender?

Note – Show a stacked bar chart

Ans 1 ->

a. ->

dataset$Fare <- (dataset$Fare - fareStats$avgFare)/fareStats$stdFare

boxplot(fareStats$avgFare ~ Fare, ,
        main = 'Fare',
        xlab = 'class',
        ylab = 'avgFare')avgFare
        
b. ->

 summary(train$Sex)

 prop.table(table(train$Sex, train$Survived))
