# Python Basics and Data Manipulation
This repository contains solutions to a Python assignment focused on fundamental programming concepts and an introduction to data manipulation using the pandas library.

---

## 1. Working with Lists
This section covers various ways to work with lists in Python, including list comprehensions for concise code.

```extract_and_apply(l, p, f)```:
Extracts elements from a list l that satisfy a predicate p and then applies a function f to each of those elements. The provided solution uses a single-line list comprehension for efficiency.

```concatenate(seqs)```:
Concatenates a list of sequences into a single flat list using a nested list comprehension.

```transpose(matrix)```:
Transposes a 2D matrix (represented as a list of lists). The solution uses a nested list comprehension to swap rows and columns.

---

## 2. Sequence Slicing
This section demonstrates the use of sequence slicing, a powerful Python feature for creating new sequences from existing ones.

```copy(seq)```:
Creates a shallow copy of a sequence. The slice seq[:] is a common and idiomatic way to achieve this.

```all_but_last(seq)```:
Returns a new sequence containing all elements except the last one.

```every_other(seq)```:
Returns a new sequence containing every other element, starting with the first, using the optional step parameter in slicing.

---

## 3. Combinatorial Algorithms
This section focuses on using generators to efficiently produce sequences of data without storing them all in memory at once.

```prefixes(seq)``` and ```suffixes(seq)```:
Generators that yield all prefixes and suffixes of a given sequence.

```slices(seq)```:
A generator that yields all non-empty slices of a sequence.

---

## 4. Text Processing
This section covers common string manipulation and text normalization tasks.

```normalize(text)```:
Normalizes a string by converting it to lowercase and replacing all whitespace with single spaces.

```no_vowels(text)```:
Removes all vowels (a, e, i, o, u, both uppercase and lowercase) from a string.

```digits_to_words(text)```:
Extracts all digits from a string and converts them into their corresponding English words.

```to_mixed_case(name)```:
Converts a variable name from snake_case (using underscores) to camelCase (mixed case).

---

## 5. DataFrames
This section introduces the pandas library for working with DataFrames, which are tabular data structures similar to spreadsheets or SQL tables.

### 5.1 Manipulating a CSV
This part works with a CSV file from an MTurk batch to demonstrate basic DataFrame operations.

```read_file(file)```: Reads a CSV file into a pandas DataFrame.

```get_workerId_by_row(df, row)```: Retrieves a specific worker ID from the DataFrame.

```format_date(date)```: Converts a date string into a timestamp in minutes.

```convert_times(df, column)```: Applies the format_date function to a DataFrame column.

```get_work_time(df)```: Calculates the total time each worker spent on tasks based on the difference between submit and accept times.

```calculated_work_time(df)```: A more advanced function that accounts for potential overlaps in task acceptance times to get a more accurate total work time.

### 5.2 A Simple Program to Read from the Web
This part demonstrates how to read and process data from a web page using pandas.

```read_from_html(url)```: Reads HTML tables from a URL into a list of DataFrames.

```get_film_data(df_list)```: Finds a specific table (highest-grossing films) within the list of DataFrames.

```set_index(df, column)```: Sets a DataFrame column as its index.

```extract_revenue(df, column, name)```: Extracts and cleans revenue data from a string column, converting it to a numeric value in millions.

```get_dimensions(df)```: Returns the dimensions (rows, columns) of a DataFrame using the .shape attribute.
