<!-- This is the markdown template for the final project of the Building AI course, 
created by Reaktor Innovations and University of Helsinki. 
Copy the template, paste it to your GitHub README and edit! -->

# Fabric Ordering

Final project for the Building AI course

## Summary

I have a company that sells performance fabric to the interior design trade. I would like to know when to order new fabric styles and colours so that the customers are fulfilled in a timely manner and I am not using too much warehouse space and capital.


## Background

Interior Designers order my fabric by the yard, in amounts ranging from one yard for a cushion to hundreds of yards for a restaurant or hotel.

The fabric comes in about 30 combinations of style and colour.

It is difficult to know when to order more fabric because
* Demand is spiky
* Lead times can be very long
* I don't know which colours and styles will be most popular
* I don't want to spend the money to buy fabric that will sit in a warehouse for a long time
* I don't want to miss out on a big order because I am out of stock


## How is it used?

The solution would be run regularly, about once a month. It would give recommendations about which colours and styles to order, and in what amounts.


## Data sources and AI methods

The data would come from
* Current supplier lead times
* Available space in the warehouse
* Customer inquiries
* Customer sales
* Views on colour and style pages on the website
* Orders

I think the best method would be to create a linear regression model with weights for each of these inputs and a threshold on the output to recommend what to buy. The model should be continously updated with the latest inputs and tested against the orders, both successful and unsuccessful.

## Challenges

The challenge I see, and the reason this human has not been able to solve this problem without machine learning is that the orders are spiky. This means that there can be a 200 yard order for one colour/style one month and then only small orders for the next month. It is difficult to predict when and where the next order will come from.


## What next?

The first thing that I would do is to create a linear regression model and assign some weights to the inputs. 

I am not sure how to turn the model into a recommendation, so I would have to research how to do this.
