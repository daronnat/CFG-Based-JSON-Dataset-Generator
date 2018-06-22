# CFG-Based-Question-Generator

JSON dataset generator written in Python3 based on Context Free Grammar rules and Cartesian products.
The goal of this script is to be able to quickly generate a dataset ready to be used with most of the machine learning libraries focused on Natural Language Understanding (NLU). The script relies on a rules.txt file easy to manipulate and modify according to your needs.

## Getting Started

To test the script, simply put the rules file and the dataset generator in the same folder, then proceed to launch the python file with the method of your choice.

### Prerequisites

* Python3.6
* The NLTK python library
* the num2word python library

## The output

If everything is working you should have a ready-to-be-used JSON dataset.
A line from the dataset should look like something like this:
```
{"text": "i am looking for a fast food restaurant", "intent": "get_restaurants", "entities": [{"start": 19, "end": 39, "value": "fast food restaurant", "entity": "food"}]},
```
Here is a description of the different elements:
* "text": contains the full query generated by the program
* "intent": indicate the kind of action/category linked to the query
* "entities": indicate the location and value of the keyword in the sentence, in the example it's "fast food restaurant"
* "entity": additional information aimed to facilitate the classification of the query 

## Built With

* [Python3](https://www.python.org/) - The Python Programming Language
* [num2words](https://pypi.python.org/pypi/num2words) - The num2words Python3 library
* [NLTK](http://www.nltk.org/) - The NLTK project

## Authors

* **Sylvain Daronnat** - [Sylvain Daronnat's github](https://github.com/daronnat)

## License

This project is licensed under the MIT License - see the [LICENSE.md](LICENSE.md) file for details

