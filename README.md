# final-programming-design-2026
Final: Programming Design 2026.

## 01. Define a class `SequenceGenerator` which instantiates objects with four methods `get_evens()`, `get_odds()`, `get_primes()`, and `get_fibonacci()` that return a `list` with the first `n` evens, odds, primes or integers of a Fibonacci sequence (given `n >= 2`).

- Source: <https://en.wikipedia.org/wiki/Prime_number>
- Source: <https://en.wikipedia.org/wiki/Fibonacci_sequence>

```python
class SequenceGenerator:
    """
    >>> sequence_generator = SequenceGenerator(5)
    >>> sequence_generator.get_evens()
    [0, 2, 4, 6, 8]
    >>> sequence_generator.get_odds()
    [1, 3, 5, 7, 9]
    >>> sequence_generator.get_primes()
    [2, 3, 5, 7, 11]
    >>> sequence_generator.get_fibonacci()
    [0, 1, 1, 2, 3]
    >>> sequence_generator = SequenceGenerator(7)
    >>> sequence_generator.get_evens()
    [0, 2, 4, 6, 8, 10, 12]
    >>> sequence_generator.get_odds()
    [1, 3, 5, 7, 9, 11, 13]
    >>> sequence_generator.get_primes()
    [2, 3, 5, 7, 11, 13, 17]
    >>> sequence_generator.get_fibonacci()
    [0, 1, 1, 2, 3, 5, 8]
    """
    ### BEGIN SOLUTION
    
    ### END SOLUTION
```

## 02. Define a function `factorial()` which returns the result of $n!$.

Source: <https://en.wikipedia.org/wiki/Factorial>

```python
def factorial(n: int) -> int:
    """
    >>> factorial(0)
    1
    >>> factorial(1)
    1
    >>> factorial(2)
    2
    >>> factorial(3)
    6
    >>> factorial(4)
    24
    """
    ### BEGIN SOLUTION
    
    ### END SOLUTION
```

## 03. Define a function `get_optimal_change()` in New Taiwan Dollar currency system. By saying "optimal" means the cashier has enough amount of all currency amounts in coins and notes, and the cashier strives for giving customer as few as possible.

```python
def get_optimal_change(sale_price: int, paid: int) -> dict:
    """
    >>> get_optimal_change(35, 50)
    {500: 0, 100: 0, 50: 0, 10: 1, 5: 1, 1: 0}
    >>> get_optimal_change(69, 100)
    {500: 0, 100: 0, 50: 0, 10: 3, 5: 0, 1: 1}
    >>> get_optimal_change(124, 150)
    {500: 0, 100: 0, 50: 0, 10: 2, 5: 1, 1: 1}
    >>> get_optimal_change(124, 200)
    {500: 0, 100: 0, 50: 1, 10: 2, 5: 1, 1: 1}
    >>> get_optimal_change(124, 500)
    {500: 0, 100: 3, 50: 1, 10: 2, 5: 1, 1: 1}
    >>> get_optimal_change(124, 1000)
    {500: 1, 100: 3, 50: 1, 10: 2, 5: 1, 1: 1}
    >>> get_optimal_change(1124, 1500)
    {500: 0, 100: 3, 50: 1, 10: 2, 5: 1, 1: 1}
    >>> get_optimal_change(1124, 2000)
    {500: 1, 100: 3, 50: 1, 10: 2, 5: 1, 1: 1}
    """
    ### BEGIN SOLUTION
    
    ### END SOLUTION
```

## 04. Define a function `rotate_character()` which rotates a character with the 13th letter after it.

Source: <https://en.wikipedia.org/wiki/ROT13>

```python
def rotate_character(x: str) -> str:
    """
    >>> rotate_character("A")
    'N'
    >>> rotate_character("B")
    'O'
    >>> rotate_character("L")
    'Y'
    >>> rotate_character("M")
    'Z'
    >>> rotate_character("a")
    'n'
    >>> rotate_character("b")
    'o'
    >>> rotate_character("l")
    'y'
    >>> rotate_character("m")
    'z'
    """
    ### BEGIN SOLUTION
    
    ### END SOLUTION
```

## 05. Define a function `rotate_sentence()` which rotates a sentence with ROT13.

Source: <https://en.wikipedia.org/wiki/ROT13>

```python
def rotate_sentence(x: str) -> str:
    """
    >>> rotate_sentence("Abj vf orggre guna arire.")
    'Now is better than never.'
    >>> rotate_sentence("Now is better than never.")
    'Abj vf orggre guna arire.'
    >>> rotate_sentence("Rkcyvpvg vf orggre guna vzcyvpvg.")
    'Explicit is better than implicit.'
    >>> rotate_sentence("Explicit is better than implicit.")
    'Rkcyvpvg vf orggre guna vzcyvpvg.'
    """
    ### BEGIN SOLUTION
    
    ### END SOLUTION 
```

## 06. Define a class `Rot13` which instantiates objects with 2 methods `rotate_character()` and `rotate_sentence()`.

Source: <https://en.wikipedia.org/wiki/ROT13>

```python
class Rot13:
    """
    >>> rot13 = Rot13()
    >>> rot13.rotate_character("A")
    'N'
    >>> rot13.rotate_character("B")
    'O'
    >>> rot13.rotate_character("L")
    'Y'
    >>> rot13.rotate_character("M")
    'Z'
    >>> rot13.rotate_character("a")
    'n'
    >>> rot13.rotate_character("b")
    'o'
    >>> rot13.rotate_character("l")
    'y'
    >>> rot13.rotate_character("m")
    'z'
    >>> rot13.rotate_sentence("Abj vf orggre guna arire.")
    'Now is better than never.'
    >>> rot13.rotate_sentence("Now is better than never.")
    'Abj vf orggre guna arire.'
    >>> rot13.rotate_sentence("Rkcyvpvg vf orggre guna vzcyvpvg.")
    'Explicit is better than implicit.'
    >>> rot13.rotate_sentence("Explicit is better than implicit.")
    'Rkcyvpvg vf orggre guna vzcyvpvg.'
    """
    ### BEGIN SOLUTION
    
    ### END SOLUTION
```

## 07. Given a plain text file `friends.txt` in working directory, define a class `Friends` with 2 methods `get_actor()` and `get_character()`.

```python
class Friends:
    """
    >>> friends = Friends()
    >>> friends.get_actor("Rachel Green")
    'Jennifer Aniston'
    >>> friends.get_actor("Monica Geller")
    'Courteney Cox'
    >>> friends.get_actor("Phoebe Buffay")
    'Lisa Kudrow'
    >>> friends.get_character("Jennifer Aniston")
    'Rachel Green'
    >>> friends.get_character("Courteney Cox")
    'Monica Geller'
    >>> friends.get_character("Lisa Kudrow")
    'Phoebe Buffay'
    """
    ### BEGIN SOLUTION
    
    ### END SOLUTION
```

## 08. Define a function `import_mlb_teams_json()` which imports `mlb_teams.json` in working directory.

```python
def import_mlb_teams_json() -> list:
    """
    >>> mlb_teams = import_mlb_teams_json()
    >>> type(mlb_teams)
    list
    >>> len(mlb_teams)
    30
    """
    ### BEGIN SOLUTION
    
    ### END SOLUTION
```

## 09. Define a function `find_teams_ballpark()` which returns the ballpark given team name and `mlb_teams.json` in working directory.

```python
def find_teams_ballpark(team: str) -> str:
    """
    >>> find_teams_ballpark("Boston Red Sox")
    'Fenway Park'
    >>> find_teams_ballpark("New York Yankees")
    'Yankee Stadium'
    >>> find_teams_ballpark("Los Angeles Dodgers")
    'Dodger Stadium'
    """
    ### BEGIN SOLUTION
    
    ### END SOLUTION
```

## 10. Define a function `find_ballpark_full_address()` which returns the ballpark's full address in the format of `address, city, state, country` separated by comma given team name and `mlb_teams.json` in working directory.

```python
def find_ballpark_full_address(team: str) -> str:
    """
    >>> find_ballpark_full_address("Boston Red Sox")
    '4 Jersey Street, Boston, MA, United States'
    >>> find_ballpark_full_address("New York Yankees")
    'One East 161st Street, Bronx, NY, United States'
    >>> find_ballpark_full_address("Los Angeles Dodgers")
    '1000 Vin Scully Avenue, Los Angeles, CA, United States'
    """
    ### BEGIN SOLUTION
    
    ### END SOLUTION
```

## 11. Define a function `import_imdb_files()` which imports `movies.csv`, `release_info.csv`, `movies_directors.csv`, and `directors.csv` as Pandas DataFrames in working directory.

```python
def import_imdb_files() -> tuple:
    """
    >>> movies, release_info, movies_directors, directors = import_imdb_files()
    >>> movies.shape
    (250, 5)
    >>> release_info.shape
    (17717, 4)
    >>> movies_directors.shape
    (284, 4)
    >>> directors.shape
    (179, 3)
    """
    ### BEGIN SOLUTION
    
    ### END SOLUTION
```

## 12. Define a function `find_the_shawshank_redemption_release_info()` which returns the release information of the movie "The Shawshank Redemption".

```
                       title        country release_date
0   The Shawshank Redemption         Canada   1994-09-10
1   The Shawshank Redemption  United States   1994-09-13
2   The Shawshank Redemption  United States   1994-09-22
3   The Shawshank Redemption         Canada   1994-09-23
4   The Shawshank Redemption         Mexico   1994-09-23
..                       ...            ...          ...
63  The Shawshank Redemption          Egypt   2021-04-18
64  The Shawshank Redemption         Israel   2021-09-14
65  The Shawshank Redemption     Kazakhstan   2022-06-04
66  The Shawshank Redemption          China   2023-04-20
67  The Shawshank Redemption    South Korea   2024-05-08

[68 rows x 3 columns]
```

```python
def find_the_shawshank_redemption_release_info() -> pd.core.frame.DataFrame:
    """
    >>> the_shawshank_redemption_release_info = find_the_shawshank_redemption_release_info()
    >>> the_shawshank_redemption_release_info.shape
    (68, 3)
    """
    ### BEGIN SOLUTION
    
    ### END SOLUTION
```

## 13. Define a function `find_the_shawshank_redemption_release_info_in_taiwan()` which returns the release information of the movie "The Shawshank Redemption" in Taiwan.

```python
def find_the_shawshank_redemption_release_info_in_taiwan(nth_release: str) -> str:
    """
    >>> find_the_shawshank_redemption_release_info_in_taiwan("1st") # First release
    "1995-03-10"
    >>> find_the_shawshank_redemption_release_info_in_taiwan("2nd") # Re-release
    "2020-03-13"
    """
    ### BEGIN SOLUTION
    
    ### END SOLUTION
```

## 14. Define a function `find_movies_directed_by_nolan_spielberg()` which finds out movies directed by Christopher Nolan and Steven Spielberg. Select specified columns showing movie's title and director's name given `movies.csv`, `movies_directors.csv`, and `directors.csv` in working directory.

```
             director                               title
0   Christopher Nolan                     The Dark Knight
1   Christopher Nolan                           Inception
2   Christopher Nolan                        Interstellar
3   Christopher Nolan                        The Prestige
4   Christopher Nolan                             Memento
5   Christopher Nolan               The Dark Knight Rises
6   Christopher Nolan                         Oppenheimer
7   Christopher Nolan                       Batman Begins
8    Steven Spielberg                    Schindler's List
9    Steven Spielberg                 Saving Private Ryan
10   Steven Spielberg             Raiders of the Lost Ark
11   Steven Spielberg  Indiana Jones and the Last Crusade
12   Steven Spielberg                       Jurassic Park
13   Steven Spielberg                 Catch Me If You Can
14   Steven Spielberg                                Jaws
```

```python
def find_movies_directed_by_nolan_spielberg() -> pd.core.frame.DataFrame:
    """
    >>> movies_directed_by_nolan_spielberg = find_movies_directed_by_nolan_spielberg()
    >>> type(movies_directed_by_nolan_spielberg)
    pandas.core.frame.DataFrame
    >>> movies_directed_by_nolan_spielberg.shape
    (15, 2)
    """
    ### BEGIN SOLUTION
    
    ### END SOLUTION
```

## 15. Define a function `find_movies_with_multiple_directors()` which finds out movies directed by multiple directors. Select specified columns showing movie's title and director's name given `movies.csv`, `movies_directors.csv`, and `directors.csv` in working directory.

```
                                  title               director
0                               Aladdin            John Musker
1                               Aladdin           Ron Clements
2                     Avengers: Endgame          Anthony Russo
3                     Avengers: Endgame              Joe Russo
4                Avengers: Infinity War          Anthony Russo
5                Avengers: Infinity War              Joe Russo
6                           City of God     Fernando Meirelles
7                           City of God             Kátia Lund
8                                  Coco          Adrian Molina
9                                  Coco            Lee Unkrich
10                                Fargo             Ethan Coen
11                                Fargo              Joel Coen
12                         Finding Nemo         Andrew Stanton
13                         Finding Nemo            Lee Unkrich
14                   Gone with the Wind           George Cukor
15                   Gone with the Wind               Sam Wood
16                   Gone with the Wind         Victor Fleming
17             How to Train Your Dragon          Chris Sanders
18             How to Train Your Dragon           Dean DeBlois
19                           Inside Out            Pete Docter
20                           Inside Out      Ronnie Del Carmen
21                                Klaus  Carlos Martínez López
22                                Klaus          Sergio Pablos
23                  Like Stars on Earth             Aamir Khan
24                  Like Stars on Earth            Amole Gupte
25                       Monsters, Inc.        David Silverman
26                       Monsters, Inc.            Lee Unkrich
27                       Monsters, Inc.            Pete Docter
28      Monty Python and the Holy Grail          Terry Gilliam
29      Monty Python and the Holy Grail            Terry Jones
30               No Country for Old Men             Ethan Coen
31               No Country for Old Men              Joel Coen
32                          Ratatouille              Brad Bird
33                          Ratatouille            Jan Pinkava
34                  Singin' in the Rain             Gene Kelly
35                  Singin' in the Rain          Stanley Donen
36  Spider-Man: Across the Spider-Verse     Joaquim Dos Santos
37  Spider-Man: Across the Spider-Verse     Justin K. Thompson
38  Spider-Man: Across the Spider-Verse            Kemp Powers
39    Spider-Man: Into the Spider-Verse        Bob Persichetti
40    Spider-Man: Into the Spider-Verse           Peter Ramsey
41    Spider-Man: Into the Spider-Verse         Rodney Rothman
42                     The Big Lebowski             Ethan Coen
43                     The Big Lebowski              Joel Coen
44                          The General          Buster Keaton
45                          The General         Clyde Bruckman
46                     The Intouchables        Olivier Nakache
47                     The Intouchables          Éric Toledano
48                        The Lion King            Rob Minkoff
49                        The Lion King           Roger Allers
50                           The Matrix         Lana Wachowski
51                           The Matrix        Lilly Wachowski
52                     The Wizard of Oz             King Vidor
53                     The Wizard of Oz         Victor Fleming
54                                   Up           Bob Peterson
55                                   Up            Pete Docter
```

```python
def find_movies_with_multiple_directors() -> pd.core.frame.DataFrame:
    """
    >>> movies_with_multiple_directors = find_movies_with_multiple_directors()
    >>> type(movies_with_multiple_directors)
    pandas.core.frame.DataFrame
    >>> movies_with_multiple_directors.shape
    (56, 2)
    """
    ### BEGIN SOLUTION
    
    ### END SOLUTION
```