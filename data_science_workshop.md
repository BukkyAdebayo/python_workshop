Python for Data Science Workshop
Teacher's Outline


[Warmup] 10 minutes (as people are coming in to sit)
Give them "The Task At Hand" before sharing the notebook. Walk around to assess where students are in terms of python. Might have 1 or 2 very good (using pandas), but most will likely struggle. Assure them after time passed that it's not important if they finished or not, and it'll be walked through.

[Intros and Objectives] 15 minutes (25)
Get names, introduce yourself and goals for the day (put on board)
Walk through the two solutions by talking through the code.
At `str(age) not in age_counter` ask a student to explain (they should notice it is similar to the gender part) to see if they're getting it or not.
After explaining pandas one, ask about preferences (who likes version 1? version 2?)

[Anaconda|ipython|notebook review] 10 minutes (35)
Inform students more about what they installed. Walk everyone through the steps to get jupyter notebook running on their machine. At the end, good chance to see if anyone installed python3, as that will change a couple things for them (like int division)

[Let's Practice] 10 minutes (45)
Review "commenting through the code" by doing that with them

1. Add a comment above each line of code in the first cell
2. write a short markdown cell of three things they learned from that cell:
3. I usually go with
    4. two numeric types: float and int
    5. dividing integers will truncate and return an int, floats will return floats
    6. use `help()` to get information about an object in python

[Basic Data Types] 15 minutes (60)
Students practice "commenting through the code" on their own. they should type out the code, write comments. walk around and observe.
Use the last 5 minutes of the 15 to have students explain chunks of code
Then, use a couple minutes to have students write what they learned

(Note, i used to have a section on dictionaries and functions, but it was removed. You could easily add one back in).

[Libraries for Data Science] 5 minutes (65)
Just talk about what each of these libraries are. Let students know we'll really just be using pandas, as that's 99% of the job anyway (in code, at least).

- __```numpy```__ - scientific computation library. Has a really powerful matrix datatype that is the basis of the ```pandas``` library and contains the functionality of that 
- __```scipy```__ - a library built on the numpy library but has more advaced linear algebra and numerical algorithm functions
- __```pandas```__ - We will be working with the for most of the day. It's built on numpy. A library for data analysis
- __```matplotlib```__ - The python 2D plotting library
- __```statsmodel```__ - A library for statistical models and testing
- __```scikitlearn```__ - Library for machine learning
- __```nltk```__ - Library for natural language processing



[pandas and object oriented programming] 15 minutes (80)
Walk students through how to read `<class 'pandas.core.frame.DataFrame'>` I like to pull up the github for pandas and show the folders and files it fits into:

pandas/core/frame.py -> class DataFrame():

Talk about the two primary datatypes in pandas: DataFrame and Series.
Then explain the difference between an object variable and function().

[Type exploration] 15 minutes (95)
Show them how to do the following cell:

```python
# example:
nyt.dtypes?
print nyt.dtypes
print type(nyt.dtypes)
```

They'll use the rest of the time to go through the rest of the functions below.

[Early Data Exploration] 30 minutes (125)

Show them how to easily download the datasets chickwts, msleep, cars93. I'd remove the rest. infert and poison seem too negative and less people are interested; Baseball is very large, requires prior knowledge, and not good for in class, but good to use outside of class.

They do the instructions; before lunch ask a couple students to explain what each data set is about, what columns are available. any points of interest they might want to further explore later, etc

[Lunch Break] 30 minutes (155)

[Data Munging basics] 10 minutes (165)
Have this printed cell presented (on the screen) as students come back in and pose the question while they settle in: what's interesting about this "view"?
They should see the signed_in data has no gender data.

Filter -> Pivot/Agg 15 minutes each (225)

I generally do micro lessons here. explain the idea, ask around about why this would be useful, show an example, guided practice on the fly (what would the code look like if I wanted to do X? ask a student who's keeping up well), independent practice on the fly (more questions, but let students work on them for a minute)

I spend the MOST time on apply because it is a very thick concept--sometimes up to 30 minutes. I sometimes skip over selecting rows/etc as it's relatively intuitive. I don't always go over pivot tables.

[plotting] 15 minutes (240)
I only do this section if you are way ahead of schedule.

[independent practice] 30 minutes (270)

Students in small groups work in more detail on one of the data sets from earlier (cars, sleep, chkweights). I push them to write at least three things they're interested in exploring/getting answers about before actually writing code. (I call this "writing with purpose," if that makes sense).

[wrapup] 15 minutes (285)

Students in small groups talk about the dataset they worked on with the rest of the class and some "next steps," what they are interested in doing more of.

think-pair-share
At the tail end ask students to write their final markdown notetaker (write about what you learned today). Have students share with their neighbor then share with the class.

Go over next steps and say bye!