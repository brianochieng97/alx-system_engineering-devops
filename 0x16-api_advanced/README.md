# Solutions API advanced project

- Querying Reddit API's.

## Tests :

* [tests](./tests): tests dir

## Function Prototypes :

Prototypes functions for the project:

| File           | Prototype                               |
| -------------- | --------------------------------------- |
| `0-subs.py`    | `def number_of_subscribers(subreddit)`  |
| `1-top_ten.py` | `def top_ten(subreddit)`                |
| `2-recurse.py` | `def recurse(subreddit, hot_list=[])`   |
| `100-count.py` | `def count_words(subreddit, word_list)` |

## Tasks 

* **0. How many subs?**
  * [0-subs.py](./0-subs.py): A Python function that queries the Reddit API and returns the number of subscribers (not active users, total subscribers) for a given subreddit
  * Returns `0` if an invalid subreddit is given.

* **1. Top Ten**
  * [1-top_ten.py](./1-top_ten.py): A Python function that queries the Reddit API and prints the titles of the first 10 hot posts listed for a given subreddit.
  * Prints `None` if an invalid subreddit is given.

* **2. Recurse it!**
  * [2-recurse.py](./2-recurse.py): A Recursive function that recursively returns a
  list of titles for all hot articles on a given subreddit.
  * Returns `None` if no results are found on the given subreddit.
  * The Reddit API uses pagination for separating pages of responses.

* **3. Count it!**
  * [100-count.py](./100-count.py): A recursive function that queries the Reddit API, parses the title of all hot articles, and prints a sorted count of given keywords (case-insensitive, delimited by spaces. Javascript should count as javascript, but java should not).
  * Keywords are case-insensitive and delimited by spaces.
  * Results are printed in descending order by the count.
  * Words with identical counts are sorted alphabetically (ascending from A to Z).
  * Words with no matches are skipped and not printed.
  * Words must be printed in lowercase.
  * Results are based on the number of times a keyword appears - ie.,
  `java java java` counts as three separate instances of `java`.
  * Print nothing if posts don't match or the subreddit is invalid.
