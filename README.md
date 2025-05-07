# Python SkillBuilder Summary

### 📚 Table of Contents

- [SkillBuilder 1: The Power of Python](#-skillbuilder-1-the-power-of-python)
- [SkillBuilder 2: Logic, Lists & Loops](#-skillbuilder-2-logic-lists--loops)
- [SkillBuilder 3: Dictionaries and Conditional Logic](#-skillbuilder-3-dictionaries-and-conditional-logic)
- [SkillBuilder 4: Building on the Basics](#-skillbuilder-4-building-on-the-basics)
- [SkillBuilder 5: Introduction to Pandas](#-skillbuilder-5-introduction-to-pandas)
- [SkillBuilder 6: Pandas and Visualization](#-skillbuilder-6-pandas-and-visualization)
- [SkillBuilder 7: Pandas and Filtering Data](#skillbuilder-7-pandas-and-filtering-data)
- [SkillBuilder 8: Cleaning and Summarizing Data](#skillbuilder-8-cleaning-and-summarizing-data)
- [SkillBuilder 9: Pandas and Joining Data](#skillbuilder-9-pandas-and-joining-data)



# 🧠 SkillBuilder 1: The Power of Python

Welcome to your first SkillBuilder! This section introduces foundational Python syntax — the building blocks you'll use again and again as you grow as a coder.

You'll learn how to print output, work with strings and numbers, name variables effectively, and format your output in style. ✨

---

## 🖨️ **The `print()` Function**

The `print()` function displays output in the console so you can see what your code is doing.

```python
print("My name is Bodhi!")
print("Hello", "World")
```

✅ **Explore more:** [W3Schools - Python Output](https://www.w3schools.com/python/python_output.asp)

---

## 🧵 **Data Type: Strings**

A **string** (`str`) is a sequence of characters inside single (`'`), double (`"`), or triple quotes (`'''` or `"""` for multi-line strings).

> 💡 Opening and closing quotes must match.
> 
> 
> 🔠 **Casing matters** – `"A"` is not the same as `"a"`.
> 

```python
str1 = 'Hello'
str2 = "World"
str3 = '''This is a
multi-line string.'''

greeting = str1 + " " + str2  # Concatenation
length = len(greeting)        # Length of string

print(greeting)  # Output: Hello World
print(length)    # Output: 11
print(str3)      # Ouput: This is a
								 # multi-line string
```

> 🧠 Strings are sequences — you can access individual characters with indexing:
> 

```python
text = "hello"
print(text[0])   # Output: h
print(text[-1])  # Output: o
```

> 💥 Indexing beyond the length causes an error:
> 

```python
print(text[10])  # IndexError: string index out of range
```

### ✂️ **Slicing Strings**

You can extract parts of a string using **slicing**:

```python
word = "hello world"

print(word[0:5])   # Output: hello
print(word[:5])    # Output: hello
print(word[6:])    # Output: world
print(word[-5:])   # Output: world

```

Use `string[start:stop]` → start is **inclusive**, stop is **exclusive**.

Add a **step** for extra control:

```python
print(word[::2])   # Output: hlowrd
```

✅ **Explore more:** [W3Schools - Python Strings](https://www.w3schools.com/python/python_strings.asp)

---

## ➕ **Data Type: Numbers**

Python handles different numeric types:

- `int` → whole numbers (5, -3)
- `float` → decimal numbers (3.14, -0.5)
- `complex` → numbers with real + imaginary parts (2 + 3j)

```python
x = 10      # Integer
y = 3.14    # Float
z = 2 + 3j  # Complex number
```

✅ **Explore more:** [W3Schools - Python Numbers](https://www.w3schools.com/python/python_numbers.asp)

---

## 🗣️ **Declaring and Using Variables**

Variables are created using `=`.

Use **descriptive, snake_case names** (lowercase + underscores):

```python
name = "Bob"
age = 30
height = 5.9
favorite_color = "red"
favorite_potato = "sweet"

print("Name:", name)
print("Age:", age)
print("Height:", height, "ft")
print("Favorite Color:", favorite_color)
print("Favorite potato type:", favorite_potato)
```

> ⚠️ Variables are case-sensitive and can't start with numbers.
> 
> 
> 🚫 Avoid spaces, hyphens, or reserved words (like `print`, `def`, `for`).
> 

✅ **Explore more:** [W3Schools - Python Variables](https://www.w3schools.com/python/python_variables.asp).

---

## 🔠 **String Functions and Methods**

Some useful string methods:

```python
word = "banana"

print(word.upper())        # BANANA
print(word.capitalize())   # Banana
print(word.count("a"))     # 3
print(word.find("na"))     # 2
print(word.replace("a", "o"))  # bonono
```

✅ **Explore more:** [W3Schools - Python String Methods](https://www.w3schools.com/python/python_ref_string.asp)

---

## ✨ **f-Strings (Formatted Strings)**

**f-strings** let you embed variables inside strings cleanly:

```python
name = "Charlie"
age = 28

print(f"My name is {name} and I am {age} years old.")
print(f"Next year, I will be {age + 1} years old.")
```

🚫 Older ways (less readable):

```python
print("My name is " + name + " and I am " + str(age) + " years old.")
```

✅ **Explore more:** [W3Schools - f-Strings](https://www.w3schools.com/python/python_string_formatting.asp)

---

## 🧪 **Bonus: Jupyter Notebook Tips**

Jupyter Notebooks are great for experimenting with Python code. Some handy shortcuts:

- ▶️ **Run a cell:** `Shift + Enter`
- ➕ **Add cell below:** `B`
- 🔼 **Add cell above:** `A`
- ❌ **Delete a cell:** `D` `D`
- 📝 **Edit a cell:** `Enter`
- 🧪 **Command vs Edit Mode:** `Esc` for command mode, `Enter` to edit
- 💬 **Markdown notes:** Change a cell to Markdown with `M` → use `#` for headers, `bold*`,  for lists

> 💡 Pro Tip: Use Markdown cells to explain your thought process or annotate code for clarity.
> 

✅ **Explore more:** [Jupyter Notebook Docs](https://jupyter-notebook.readthedocs.io/en/stable/examples/Notebook/Notebook%20Basics.html)

---

🎉 **Recap:** You’ve learned how to:

- Use `print()` for output
- Work with strings & numbers
- Declare variables with good names
- Format output cleanly with f-strings

You’re building solid Python foundations! 🏗️

---

# 🧠 SkillBuilder 2: Logic, Lists & Loops

This SkillBuilder dives into **logic, lists, loops, and boolean expressions** — the core building blocks that let Python make decisions and repeat tasks.

---

## ✅ **Booleans**

A **Boolean** is a data type with only two possible values: `True` or `False`. You'll use these in conditions and comparisons.

```python
is_raining = True
is_sunny = False
```

Comparison operations return Boolean values:

```python
print(5 > 3)      # True
print(10 == 5)    # False
print("a" != "b")  # True
```

> 🔗 Learn more: [W3Schools - Python Booleans](https://www.w3schools.com/python/python_booleans.asp)
> 

---

## ⚙️ **Built-In Functions**

Python includes many **built-in functions** that work across data types:

```python
print(len("hello"))     # 5
print(max([1, 5, 3]))   # 5
print(round(3.14159, 2))  # 3.14
```

> 🔗 Explore more: [W3Schools - Built-in Functions](https://www.w3schools.com/python/python_ref_functions.asp)
> 

---

## 🔧 **Methods**

A **method** is a function tied to a specific data type (like strings or lists).

### 🧵 **String Methods**

```python
text = "python"
print(text.upper())        # PYTHON
print(text.capitalize())   # Python
print(text.startswith("p"))  # True
```

### 📚 **List Methods**

```python
my_list = [1, 2, 3]
my_list.append(4)       # Adds 4 to the end
my_list.remove(2)       # Removes the first occurrence of 2
print(my_list)          # [1, 3, 4]
```

> 🧠 Quick reference: [W3Schools - String Methods](https://www.w3schools.com/python/python_ref_string.asp) | [W3Schools - List Methods](https://www.w3schools.com/python/python_lists_methods.asp)
> 

---

## ➗ **Numeric Operators**

Python supports standard math operators:

- Addition: `+`
- Subtraction:
- Multiplication:
- Division: `/`
- Floor Division: `//`
- Modulo: `%` (remainder)
- Exponentiation: `*`

```python
print(7 // 2)  # 3
print(7 % 2)   # 1
```

> ➕ Learn more: [W3Schools - Python Operators](https://www.w3schools.com/python/python_operators.asp)
> 

---

## 📚 **Lists**

A **list** is an ordered collection of items.

```python
fruits = ["apple", "banana", "cherry"]
print(fruits[0])       # apple
print(len(fruits))     # 3
```

Lists can hold **any data type — even other lists**:

```python
mixed = [1, "hello", True, [2, 3]]
```

### ✂️ **Slicing Lists**

You can access parts of a list using **slicing**:

```python
fruits = ["apple", "banana", "cherry", "date", "elderberry"]

print(fruits[1:4])   # ['banana', 'cherry', 'date']
print(fruits[:3])    # ['apple', 'banana', 'cherry']
print(fruits[2:])    # ['cherry', 'date', 'elderberry']
print(fruits[-2:])   # ['date', 'elderberry']
```

Slicing pattern: `list[start:stop]` → start is **inclusive**, stop is **exclusive**.

> 📘 Learn more: [W3Schools - Python Lists](https://www.w3schools.com/python/python_lists.asp)
> 

---

## 🔁 **For Loops**

Use a `for` loop to **iterate over items** in a sequence:

```python
fruits = ["apple", "banana", "cherry"]

for fruit in fruits:
    print(fruit)

# Output:
# apple
# banana
# cherry
```

Or loop using `range()`:

```python
for i in range(5):
    print(i)

# Output:
# 0
# 1
# 2
# 3
# 4
```

> 🔄 Loop deeper: [W3Schools - Python For Loops](https://www.w3schools.com/python/python_for_loops.asp)
> 

---

🎉 **Recap:** You’ve learned how to:

- Use Boolean logic for decision making
- Use built-in functions & methods
- Work with lists & slices
- Perform numeric operations
- Automate repetition with `for` loops

These tools let your code **think and repeat!** 🎉

---

# 🧠 SkillBuilder 3: Dictionaries and Conditional Logic

## 📖 **Dictionaries**

A **dictionary** (`dict`) is a collection of **key-value pairs**.

Unlike lists (which are ordered), dictionaries store values using **keys** for quick lookup.

A dictionary uses `{}` to store keys and values separated by a colon `:`.

```python
dict = {
    "key": value
}
```

Think of **keys** like labels, and **values** as the actual data.

To access a value, use `dict["key"]`.

---

### 🧾 **Simple Dictionary Example**

```python
person = {
    "name": "Mary",
    "age": 30,
    "city": "Buffalo"
}

print(person["name"])  # Output: Mary
print(person["age"])   # Output: 30
```

✅ **Explore more:** [W3Schools - Python Dictionaries](https://www.w3schools.com/python/python_dictionaries.asp)

---

### 🏗️ **Complex Dictionary (Nested Lists & Dictionaries)**

Dictionaries can store **lists** and even **other dictionaries**!

```python
company = {
    "name": "TechCorp",
    "employees": [
        {"id": 1, "name": "Hayden", "role": "Developer"},
        {"id": 2, "name": "Ianne", "role": "Designer"}
    ],
    "location": {
        "city": "Austin",
        "state": "TX"
    }
}

print(company["name"])                 # Output: TechCorp
print(company["employees"][0]["name"]) # Output: Hayden
print(company["employees"][1]["id"])   # Output: 2
print(company["location"]["city"])     # Output: Austin
```

---

### 🔄 **`for` Loops with Dictionaries**

### 🗝️ **Loop through keys**

```python
person = {
    "name": "Mary",
    "age": 30,
    "city": "Buffalo"
}

for key in person:
    print(key)

# Output:
# name
# age
# city
```

### 🗝️➡️ **Loop through keys & values**

```python
for key, value in person.items():
    print(f"{key}: {value}")
    
# Output:
# name: Mary
# age: 30
# city: Buffalo
```

### 📦 **Loop through values**

```python
for value in person.values():
    print(value)
    
# Output:
# Mary
# 30
# Buffalo
```

✅ **Explore more:** [W3Schools - Python Looping Dictionaries](https://www.w3schools.com/python/python_dictionaries_loop.asp)

---

## 🚦 **Conditionals (`if`, `elif`, `else`)** [¶](https://chatgpt.com/c/681b6440-a23c-8010-aec4-c8bdad6af073#%F0%9F%9A%A6--Conditionals-(if,-elif,-else)--)

Conditional logic lets your code make decisions based on whether something is `True` or `False`.

✅ Keywords:

- `if` → checks a condition
- `elif` → "else if" (another condition)
- `else` → runs if nothing above is `True`

```python
is_dog_hungry = True

if is_dog_hungry:
    print("You need to feed your dog.")
else:
    print("Your dog does not want to eat.")
    
# Output: You need to feed your dog.
```

### ❗ **`not` Operator**

`not` reverses a condition.

```python
is_raining = False

if not is_raining:
    print("You don't need an umbrella!")
else:
    print("Take an umbrella!")
    
# Output: You don't need an umbrella!
```

✅ **Explore more:** [W3Schools - Python Conditions](https://www.w3schools.com/python/python_conditions.asp)

---

### 🔍 **Comparison Operators**

| Operator | Meaning | Example | Result |
| --- | --- | --- | --- |
| == | Equal to | 5 == 5 | True |
| != | Not equal to | 5 != 3 | True |
| > | Greater than | 10 > 5 | True |
| < | Less than | 5 < 10 | True |
| >= | Greater or equal | 7 >= 7 | True |
| <= | Less or equal | 3 <= 5 | True |

```python
speed_limit = 25
car_speed = 35

if car_speed > speed_limit:
    print("You are going over the speed limit!")
elif car_speed == speed_limit:
    print("You are going the speed limit.")
else:
    print("You are going under the speed limit.")
    
# Output: You are going over the speed limit!
```

✅ **Explore more:** [W3Schools - Python Operators](https://www.w3schools.com/python/python_operators.asp)

---

## 📋 **List Comprehension**

List comprehensions create or modify lists **efficiently**.

```python
words = ["apple", "banana", "cherry"]
uppercase_words = [word.upper() for word in words]

print(uppercase_words)  # Output: ['APPLE', 'BANANA', 'CHERRY']
```

You can add conditions inside a list comprehension:

```python
words = ["apple", "banana", "cherry", "date"]
words_with_a = [word for word in words if "a" in word]

print(words_with_a)  # Output: ['apple', 'banana', 'date']

```

✅ **Explore more:** [W3Schools - Python List Comprehension](https://www.w3schools.com/python/python_lists_comprehension.asp)

---

🎉 **Recap:** In this SkillBuilder, you learned how to work with **dictionaries**, including accessing values, looping through keys and values, and building nested data structures. You also practiced using **conditional logic** to make decisions in code, learned key **comparison operators**, and wrote **list comprehensions** to create powerful one-liners.

✅ With these tools, you’re ready to structure data, check conditions, and write more efficient, readable Python code! 🚀

---

# 🧠 SkillBuilder 4: Building on the Basics

This SkillBuilder introduces **functions**, **while loops**, and the powerful **`zip()` function** — giving you tools to organize, repeat, and combine data in Python!

---

## ✍️ **Writing Our Own Functions**

You can create your own function using the `def` keyword.

✅ A function **must be called by its name** to run.

```python
def greet():
    print("Hello, welcome to Python!")

# Calling the function
greet()  # Output: Hello, welcome to Python!
```

👉 Functions can take **parameters** (inputs) to make them more flexible:

```python
def greet(name):
    print(f"Hello, {name}!")

# Calling with different inputs
greet("Ianne")   # Output: Hello, Ianne!
greet("Hayden")  # Output: Hello, Hayden!
```

✅ **Explore more:** [W3Schools - Python Functions](https://www.w3schools.com/python/python_functions.asp)

---

### 🎁 **Functions with Return Values**

Functions can **return values** so you can store or reuse the result later:

```python
def add(a, b):
    return a + b

result = add(3, 5)
print(result)  # Output: 8
```

Use `return` when you want your function to give back a value!

> 🧠 You can return any data type — numbers, strings, lists, even other functions.
> 

✅ **Explore more:** [W3Schools - Python Functions Return](https://www.w3schools.com/python/gloss_python_function_return.asp)

---

## 🔄 **`while` Loops**

A `while` loop **keeps running as long as the condition is `True`.**

🚨 Be careful of **infinite loops** — make sure something inside the loop will eventually make the condition `False`.

```python
count = 0

while count < 5:
    print(count)
    count += 1

# Output:
# 0
# 1
# 2
# 3
# 4
```

✅ **Explore more:** [W3Schools - Python While Loops](https://www.w3schools.com/python/python_while_loops.asp)

---

## 🤝 **The `zip()` Function**

The `zip()` function **combines multiple lists into pairs (or tuples)** — useful for combining related data.

```python
names = ["Alice", "Bob", "Charlie"]
ages = [25, 30, 35]

combined = zip(names, ages)
print(list(combined))  # Output: [('Alice', 25), ('Bob', 30), ('Charlie', 35)]
```

✅ You can convert a `zip` object into a `list` or loop through it directly.

✅ **Explore more:** [W3Schools - Python zip() Function](https://www.w3schools.com/python/ref_func_zip.asp)

---

### 🔄 **Looping Through `zip()`**

You can loop through zipped lists and **unpack** the pairs into variables:

```python
names = ["Alice", "Bob", "Charlie"]
ages = [25, 30, 35]

for name, age in zip(names, ages):
    print(f"{name} is {age} years old.")

# Output:
# Alice is 25 years old.
# Bob is 30 years old.
# Charlie is 35 years old.
```

✅ **Explore more:** [W3Schools - Python zip() Function](https://www.w3schools.com/python/ref_func_zip.asp)

---

🎉 **Recap:** You’ve learned how to write your own functions, return values, create loops that run until a condition is met, and combine multiple lists with `zip()`. These tools help you organize and process data like a pro! 🚀

---

# 🧠 SkillBuilder 5: Introduction to Pandas

This SkillBuilder introduces **pandas** — a powerful Python library for loading, exploring, and manipulating data for analysis or visualization.

---

### 📥 **How to Import Pandas**

By convention, pandas is imported as `pd` for short:

```python
import pandas as pd
```

✅ **Explore more:** [W3Schools - Python Pandas](https://www.w3schools.com/python/pandas/default.asp)

---

### 📄 **How to Read a CSV File with Pandas**

Use `.read_csv()` to load a CSV file into a **DataFrame** (a table-like structure):

```python
# Replace 'your_file.csv' with your actual filename
df = pd.read_csv("your_file.csv")
```

Once loaded, you can explore and analyze your data easily!

✅ **Explore more:** [W3Schools - Pandas Read CSV](https://www.w3schools.com/python/pandas/pandas_csv.asp)

---

### 🖼️ **DataFrames: Tables in Python**

A **DataFrame** is like an Excel table in Python — it holds:

- **Rows**
- **Columns**
- **Indexes**

---

### 👀 **Quick Look at the Data**

These methods give a fast preview of your DataFrame:

```python
df.head()     # First 5 rows
df.head(8)    # First 8 rows
df.tail(3)    # Last 3 rows
df.sample(5)  # Random 5 rows
```

✅ Use `.head()` to see the beginning, `.tail()` for the end, and `.sample()` for random variety.

---

### 🔢 **Indexes**

Every row in a DataFrame has an **index** (default is 0, 1, 2, ...).

```python
print(df.index)
```

✅ **Explore more:** [W3Schools - Pandas DataFrame](https://www.w3schools.com/python/pandas/pandas_dataframes.asp)

---

### 🏷️ **Accessing Columns**

```python
# One column
df["name"]

# Multiple columns
df[["name", "age"]]

# See all column names
print(df.columns)
```

---

### 📏 **Accessing Rows**

Use `.loc[]` to access rows by **index label**:

```python
df.loc[0]            # Entire row at index 0
df.loc[0, "name"]    # Value from row 0, column 'name'
```

✅ **Explore more:** [W3Schools - Pandas Indexing](https://www.w3schools.com/python/pandas/pandas_indexing.asp)

---

### 📊 **Quick Data Summary**

```python
df.info()      # Data types, non-null counts
df.describe()  # Summary stats for numeric columns
print(df.shape)  # (rows, columns)
```

✅ `.info()` → structure & types; `.describe()` → quick statistics; `.shape` → size overview.

✅ **Explore more:** [W3Schools - Pandas Data Exploration](https://www.w3schools.com/python/pandas/pandas_data_exploration.asp)

---

### ➕ **Simple Aggregations: sum, min, max**

✅ Works great for numeric columns, but **also works on strings** by concatenating them!

```python
df.sum()    # Adds up numeric columns, concatenates strings
df.min()    # Smallest value in each column
df.max()    # Largest value in each column
```

✅ Useful for a **quick check** or **summing up numeric data**.

---

### 🔧 **Aggregate Multiple Columns with `.agg()`**

You can apply different summary functions to different columns:

```python
df.agg({
    "salary": "mean",
    "age": ["min", "max", "mean"]
})

```

|  | salary | age |
| --- | --- | --- |
| mean | 56000.0 | 38.0 |
| min | 42000.0 | 25.0 |
| max | 73000.0 | 55.0 |

➡️ `.agg()` is helpful for **custom summary tables**.

✅ **Explore more:** [W3Schools - Pandas Aggregations](https://www.w3schools.com/python/pandas/pandas_aggregations.asp)

---

🎉 **Recap:** You’ve learned how to import pandas, read CSVs, preview your data, access columns/rows, and summarize your DataFrame. These are the first steps to becoming a data analyst with Python! 🚀

# 🧠 SkillBuilder 6: Pandas and Visualization

This SkillBuilder introduces how to use **Plotly Express** with **pandas DataFrames** to create beautiful, interactive visualizations — no need to manually pass lists!

---

## 🚞 **Plotly Express with Pandas DataFrames**

Plotly Express functions (like `px.line()`, `px.scatter()`, `px.histogram()`) work seamlessly with DataFrames.

✅ Instead of passing raw lists, you tell Plotly the **name of the columns** in your DataFrame, and it automatically looks up the data.

```python
import plotly.express as px

fig = px.line(
    df,            # The DataFrame
    x="day",      # Column name for x-axis
    y="sales",    # Column name for y-axis
    title="Sales Over Time"
)

fig.show()
```

✅ **Explore more:** [Plotly Express Docs](https://plotly.com/python/plotly-express/)

---

### 📍 **`px.scatter()` — Scatter Plots**

Scatter plots show the relationship between **two numeric variables** — great for spotting **patterns, clusters, or trends**.

You can add optional arguments like `color`, `size`, and `hover_name` for deeper insights.

```python
fig = px.scatter(
    df,
    x="height",
    y="weight",
    color="gender",      # Color by category
    size="income",       # Bubble size by value
    hover_name="name",   # Hover label when you mouse over
    title="Height vs Weight"
)

fig.show()
```

✅ Try removing or changing options like `color` or `size` to explore variations.

---

### 📊 **`px.histogram()` — Histogram**

Histograms show **distributions** — useful to see counts or frequency of values.

```python
fig = px.histogram(
    df,
    x="age",
    nbins=20,          # Number of bins (optional)
    color="gender",   # Color bars by category
    title="Age Distribution by Gender"
)

fig.show()
```

---

### 📈 **`px.bar()` — Bar Charts**

Bar charts are great for comparing **categories**.

```python
fig = px.bar(
    df,
    x="department",
    y="sales",
    color="region",
    title="Sales by Department by Region"
)

fig.show()
```

---

### 🗺️ **`px.choropleth()` — Maps**

If your DataFrame contains **location data**, Plotly can create geographic maps:

```python
fig = px.choropleth(
    df,
    locations="country_code",   # ISO country codes (e.g., "USA", "CAN")
    color="sales",
    title="Global Sales by Country"
)

fig.show()
```

✅ Explore map styles and projections in [Plotly Maps Docs](https://plotly.com/python/maps/)

---

## 🖼️ **Customizing Plots**

Plotly makes it easy to tweak the look of your plots:

```python
fig.update_layout(
    title_font_size=20,
    xaxis_title="Custom X Label",
    yaxis_title="Custom Y Label",
    template="plotly_dark"   # Try different themes!
)

fig.show()
```

✅ Check available themes: [Plotly Themes](https://plotly.com/python/templates/)

---

🎉 **Recap:** You've learned how to visualize DataFrames using Plotly Express functions like `px.line()`, `px.scatter()`, `px.histogram()`, and more — plus how to customize, explore, and save your visualizations. Ready to bring your data to life! 🚀

---

# 🧠 SkillBuilder 7: Pandas and Filtering Data

### 📋 **Starting DataFrame Example**

Let’s create a DataFrame for us to use!

```python
import pandas as pd

# Demo DataFrame for filtering examples
df = pd.DataFrame({
    "first_name": ["Daisy", "Elroy", "Freda", "George", "Hillary", "Isaac", "Julia"],
    "last_name": ["Doo", "Edgecomb", "Fitzgerald", "Gu", "Duff", "Ivy", "Jones"],
    "department": ["Sales", "Sales", "HR", "HR", "IT", "IT", "Marketing"],
    "phone_number": ["555-5551", "555-5552", "555-5553", "555-5554", "555-5555", "555-5556", "555-5557"],
    "gender": ["F", "M", "F", "M", "F", "M", "F"],
    "salary": [50000, 60000, 52000, 48000, 70000, 65000, 55000],
    "age": [25, 55, 33, 27, 50, 45, 29],
    "active": [True, True, True, False, True, False, True],
    "pets": [1, None, 2, None, None, 1, 0]
})
df.head()  # View first 5 rows
```

|  | first_name | last_name | department | phone_number | gender | salary | age | active | pets |
| --- | --- | --- | --- | --- | --- | --- | --- | --- | --- |
| 0 | Daisy | Doo | Sales | 555-5551 | F | 50000 | 25 | True | 1.0 |
| 1 | Elroy | Edgecomb | Sales | 555-5552 | M | 60000 | 55 | True | NaN |
| 2 | Freda | Fitzgerald | HR | 555-5553 | F | 52000 | 33 | True | 2.0 |
| 3 | George | Gu | HR | 555-5554 | M | 48000 | 27 | False | NaN |
| 4 | Hillary | Duff | IT | 555-5555 | F | 70000 | 50 | True | NaN |

---

## 🧹 **Filtering & Slicing Examples with Explanations**

### ✅ **`.loc[]` - Label-based access**

Select **rows 0-3** and columns **department to salary**:

```python
df.loc[0:3, "department":"salary"]
```

|  | department | phone_number | gender | salary |
| --- | --- | --- | --- | --- |
| 0 | Sales | 555-5551 | F | 50000 |
| 1 | Sales | 555-5552 | M | 60000 |
| 2 | HR | 555-5553 | F | 52000 |
| 3 | HR | 555-5554 | M | 48000 |

➡️ **Selecting a range by column names and row labels.**

---

### ✅ **`.iloc[]` - Position-based access**

Select **all rows** and the **first two columns**:

```python
df.iloc[:, 0:2]
```

|  | first_name | last_name |
| --- | --- | --- |
| 0 | Daisy | Doo |
| 1 | Elroy | Edgecomb |
| 2 | Freda | Fitzgerald |
| 3 | George | Gu |
| 4 | Hillary | Duff |
| 5 | Isaac | Ivy |
| 6 | Julia | Jones |

➡️ **Index-based column selection by number, not name.**

---

### 🔍 **Filtering Rows: Conditions Explained**

### ✅ **Filter: Age > 30**

Find employees **older than 30**:

```python
df[df["age"] > 30]
```

|  | first_name | last_name | department | phone_number | gender | salary | age | active | pets |
| --- | --- | --- | --- | --- | --- | --- | --- | --- | --- |
| 1 | Elroy | Edgecomb | Sales | 555-5552 | M | 60000 | 55 | True | NaN |
| 2 | Freda | Fitzgerald | HR | 555-5553 | F | 52000 | 33 | True | 2.0 |
| 4 | Hillary | Duff | IT | 555-5555 | F | 70000 | 50 | True | NaN |
| 5 | Isaac | Ivy | IT | 555-5556 | M | 65000 | 45 | False | 1.0 |

➡️ **Returns rows where age > 30.**

---

### ✅ **Filter: Age > 30 AND Active**

Find employees **older than 30 and still active**:

```python
df[(df["age"] > 30) & (df["active"] == True)]
```

|  | first_name | last_name | department | phone_number | gender | salary | age | active | pets |
| --- | --- | --- | --- | --- | --- | --- | --- | --- | --- |
| 1 | Elroy | Edgecomb | Sales | 555-5552 | M | 60000 | 55 | True | NaN |
| 2 | Freda | Fitzgerald | HR | 555-5553 | F | 52000 | 33 | True | 2.0 |
| 4 | Hillary | Duff | IT | 555-5555 | F | 70000 | 50 | True | NaN |

➡️ **Both conditions must be met (AND).**

---

## 🫧 **Removing and Renaming Columns**

### ✅ **Remove `phone_number` column**

```python
df.drop(columns=["phone_number"])
```

|  | first_name | last_name | department | gender | salary | age | active | pets |
| --- | --- | --- | --- | --- | --- | --- | --- | --- |
| 0 | Daisy | Doo | Sales | F | 50000 | 25 | True | 1.0 |
| 1 | Elroy | Edgecomb | Sales | M | 60000 | 55 | True | NaN |
| 2 | Freda | Fitzgerald | HR | F | 52000 | 33 | True | 2.0 |
| 3 | George | Gu | HR | M | 48000 | 27 | False | NaN |
| 4 | Hillary | Duff | IT | F | 70000 | 50 | True | NaN |
| 5 | Isaac | Ivy | IT | M | 65000 | 45 | False | 1.0 |
| 6 | Julia | Jones | Marketing | F | 55000 | 29 | True | 0.0 |

---

### ✅ **Rename `active` → `currently_employed`**

```python
df.rename(columns={"active": "currently_employed"})
```

|  | first_name | last_name | department | phone_number | gender | salary | age | currently_employed | pets |
| --- | --- | --- | --- | --- | --- | --- | --- | --- | --- |
| 0 | Daisy | Doo | Sales | 555-5551 | F | 50000 | 25 | True | 1.0 |
| 1 | Elroy | Edgecomb | Sales | 555-5552 | M | 60000 | 55 | True | NaN |
| 2 | Freda | Fitzgerald | HR | 555-5553 | F | 52000 | 33 | True | 2.0 |
| 3 | George | Gu | HR | 555-5554 | M | 48000 | 27 | False | NaN |
| 4 | Hillary | Duff | IT | 555-5555 | F | 70000 | 50 | True | NaN |
| 5 | Isaac | Ivy | IT | 555-5556 | M | 65000 | 45 | False | 1.0 |
| 6 | Julia | Jones | Marketing | 555-5557 | F | 55000 | 29 | True | 0.0 |

---

## 🔀 **Sorting with `.sort_values()`**

### ✅ **Sort by `age` ascending**

```python
df.sort_values(by="age")
```

|  | first_name | last_name | department | phone_number | gender | salary | age | active | pets |
| --- | --- | --- | --- | --- | --- | --- | --- | --- | --- |
| 0 | Daisy | Doo | Sales | 555-5551 | F | 50000 | 25 | True | 1.0 |
| 3 | George | Gu | HR | 555-5554 | M | 48000 | 27 | False | NaN |
| 6 | Julia | Jones | Marketing | 555-5557 | F | 55000 | 29 | True | 0.0 |
| 2 | Freda | Fitzgerald | HR | 555-5553 | F | 52000 | 33 | True | 2.0 |
| 5 | Isaac | Ivy | IT | 555-5556 | M | 65000 | 45 | False | 1.0 |
| 4 | Hillary | Duff | IT | 555-5555 | F | 70000 | 50 | True | NaN |
| 1 | Elroy | Edgecomb | Sales | 555-5552 | M | 60000 | 55 | True | NaN |

➡️ **This returns a new DataFrame sorted by `age` without changing the original.**

---

### ✅ **Sort by `age` descending**

```python
df.sort_values(by="age", ascending=False)
```

|  | first_name | last_name | department | phone_number | gender | salary | age | active | pets |
| --- | --- | --- | --- | --- | --- | --- | --- | --- | --- |
| 1 | Elroy | Edgecomb | Sales | 555-5552 | M | 60000 | 55 | True | NaN |
| 4 | Hillary | Duff | IT | 555-5555 | F | 70000 | 50 | True | NaN |
| 5 | Isaac | Ivy | IT | 555-5556 | M | 65000 | 45 | False | 1.0 |
| 2 | Freda | Fitzgerald | HR | 555-5553 | F | 52000 | 33 | True | 2.0 |
| 6 | Julia | Jones | Marketing | 555-5557 | F | 55000 | 29 | True | 0.0 |
| 3 | George | Gu | HR | 555-5554 | M | 48000 | 27 | False | NaN |
| 0 | Daisy | Doo | Sales | 555-5551 | F | 50000 | 25 | True | 1.0 |

➡️ Sorting descending shows the oldest first.

---

### ✅ **Sort by `department` (A-Z) then `age` (youngest first within each department)**

```python
df.sort_values(by=["department", "age"], ascending=[True, True])
```

|  | first_name | last_name | department | phone_number | gender | salary | age | active | pets |
| --- | --- | --- | --- | --- | --- | --- | --- | --- | --- |
| 2 | Freda | Fitzgerald | HR | 555-5553 | F | 52000 | 33 | True | 2.0 |
| 3 | George | Gu | HR | 555-5554 | M | 48000 | 27 | False | NaN |
| 6 | Julia | Jones | Marketing | 555-5557 | F | 55000 | 29 | True | 0.0 |
| 4 | Hillary | Duff | IT | 555-5555 | F | 70000 | 50 | True | NaN |
| 5 | Isaac | Ivy | IT | 555-5556 | M | 65000 | 45 | False | 1.0 |
| 0 | Daisy | Doo | Sales | 555-5551 | F | 50000 | 25 | True | 1.0 |
| 1 | Elroy | Edgecomb | Sales | 555-5552 | M | 60000 | 55 | True | NaN |

➡️ This sorts **department alphabetically first**, then by `age` inside each department.

📘 Learn more at [W3Schools - Pandas Sorting](https://www.w3schools.com/python/pandas/ref_df_sort_values.asp).

---

## ℹ️ **A Note on `inplace=True`**

By default, `.sort_values()` returns a **new sorted DataFrame** and leaves your original `df` unchanged.

If you'd like to sort **in place (modifying `df` directly)**, you can add `inplace=True`:

```python
df.sort_values(by="age", inplace=True)
```

✅ Now `df` is permanently sorted (no reassignment needed).

⚠️ **Be careful:** This cannot be undone unless you reload or copy your original data!

---

🎉 **Recap:** In this SkillBuilder, you learned how to filter and slice DataFrames using `.loc[]` and `.iloc[]`, apply conditional filters to select rows, remove and rename columns, and sort your data with `.sort_values()`. These foundational skills let you explore, clean, and organize data efficiently—giving you more control over how you view and analyze information in pandas.

---

# 🧠 SkillBuilder 8: Cleaning and Summarizing Data

In this SkillBuilder, we'll focus on cleaning messy data and summarizing insights using **pandas**. You'll learn how to handle missing values, replace incorrect data, and summarize using **groupby()**.

### 🕵️‍♂️ **Checking for Missing Data**

```python
# Check which cells are missing (returns True/False)
df.isnull()

# Count missing values per column
df.isnull().sum()

```

✅ Quickly spot missing data!

---

### 🧹 **Dropping Missing Data**

```python
# Drop rows with ANY missing values
df_cleaned = df.dropna()

# Drop columns with ANY missing values
df_cleaned_cols = df.dropna(axis=1)
```

➡️ Use `.dropna()` to remove incomplete rows/columns.

---

### 🩹 **Filling Missing Data**

```python
Fill missing values with 0
df_filled = df.fillna(0)

# Fill missing values in a specific column
df['pets'] = df['pets'].fillna(0)
```

✅ Great when you’d rather fill gaps than drop data.

---

### 🏷️ **Replacing Values**

```python
# Replace a value everywhere
df_replaced = df.replace('HR', 'Human Resources')

# Replace multiple values using a dictionary
df_replaced = df.replace({'HR': 'Human Resources', 'IT': 'Information Tech'})
```

➡️ Clean up inconsistent or incorrect labels.

---

### 👥 **Grouping Data with `.groupby()`**

```python
# Average salary per department
df.groupby('department')['salary'].mean()
```

| department | salary |
| --- | --- |
| HR | 50000.0 |
| IT | 67500.0 |
| Marketing | 55000.0 |
| Sales | 55000.0 |

✅ `.groupby()` lets you summarize data **by categories**.

---

### 📊 **Multiple Aggregations with `.agg()`**

```python
# Get min, max, mean salary by department
df.groupby('department')['salary'].agg(['min', 'max', 'mean'])

```

| department | min | max | mean |
| --- | --- | --- | --- |
| HR | 48000 | 52000 | 50000 |
| IT | 65000 | 70000 | 67500 |
| Marketing | 55000 | 55000 | 55000 |
| Sales | 50000 | 60000 | 55000 |

➡️ Use `.agg()` to calculate **multiple stats at once per group.**

---

### 🔍 **Filtering After Grouping**

```python
# Find departments where average salary > 55,000
high_salary = df.groupby('department')['salary'].mean()
high_salary[high_salary > 55000]
```

✅ You can **filter the results of a groupby** for deeper insights.

---

🎉 **Recap:** In this SkillBuilder, you learned how to detect and handle missing data, replace values for consistency, and drop incomplete rows or columns. You also practiced summarizing data using `.groupby()` and `.agg()` functions. With these skills, you're now equipped to clean and explore real-world datasets with confidence.

---

# 🧠 SkillBuilder 9: Pandas and Joining Data

In this SkillBuilder, you'll learn how to **combine DataFrames** using `merge()` and `concat()` methods in Pandas. This is useful when working with data from multiple sources or tables (like in SQL joins).

Let’s start with two simple DataFrames:

```python
# Customers DataFrame
customers = pd.DataFrame({
    "customer_id": [1, 2, 3, 4, 5, 6, 7, 8, 9, 10],
    "name": ["Alice", "Bob", "Charlie", "David", "Eva",
              "Frank", "Grace", "Hannah", "Ian", "Jade"]
})

# Orders DataFrame
orders = pd.DataFrame({
    "order_id": [101, 102, 103, 104, 105, 106, 107, 108, 109, 110],
    "customer_id": [2, 3, 3, 4, 6, 6, 11, 12, 1, 7],  # 11 & 12 are not in customers
    "order_total": [120, 85, 130, 70, 95, 150, 200, 300, 110, 50]
})
```

### 📋 **Starting DataFrames**

**Customers:**

| customer_id | name |
| --- | --- |
| 1 | Alice |
| 2 | Bob |
| 3 | Charlie |
| 4 | David |
| 5 | Eva |
| 6 | Frank |
| 7 | Grace |
| 8 | Hannah |
| 9 | Ian |
| 10 | Jade |

**Orders:**

| order_id | customer_id | order_total |
| --- | --- | --- |
| 101 | 2 | 120 |
| 102 | 3 | 85 |
| 103 | 3 | 130 |
| 104 | 4 | 70 |
| 105 | 6 | 95 |
| 106 | 6 | 150 |
| 107 | 11 | 200 |
| 108 | 12 | 300 |
| 109 | 1 | 110 |
| 110 | 7 | 50 |

---

## ✠ **Inner Join**

Keeps only the rows where the `customer_id` exists in *both* DataFrames.

```python
pd.merge(customers, orders, on="customer_id", how="inner")
```

**Result of Inner Join:**

| customer_id | name | order_id | order_total |
| --- | --- | --- | --- |
| 1 | Alice | 109 | 110 |
| 2 | Bob | 101 | 120 |
| 3 | Charlie | 102 | 85 |
| 3 | Charlie | 103 | 130 |
| 4 | David | 104 | 70 |
| 6 | Frank | 105 | 95 |
| 6 | Frank | 106 | 150 |
| 7 | Grace | 110 | 50 |

This excludes customers 11 and 12 since they don't exist in `customers`.

## ⬅️ **Left Join**

Keeps all rows from the *left* DataFrame (`customers`), even if there's no matching order.

```python
pd.merge(customers, orders, on="customer_id", how="left")
```

**Result of Left Join:**

| customer_id | name | order_id | order_total |
| --- | --- | --- | --- |
| 1 | Alice | 109 | 110 |
| 2 | Bob | 101 | 120 |
| 3 | Charlie | 102 | 85 |
| 3 | Charlie | 103 | 130 |
| 4 | David | 104 | 70 |
| 5 | Eva | NaN | NaN |
| 6 | Frank | 105 | 95 |
| 6 | Frank | 106 | 150 |
| 7 | Grace | 110 | 50 |
| 8 | Hannah | NaN | NaN |
| 9 | Ian | NaN | NaN |
| 10 | Jade | NaN | NaN |

Customers without orders have `NaN` in `order_id` and `order_total`.

## ⚝ **Union with `concat()`**

Combines rows from two DataFrames that have the same columns. This is like a SQL UNION ALL.

```python
df1 = pd.DataFrame({
    "name": ["Alice", "Bob"],
    "age": [25, 30]
})

df2 = pd.DataFrame({
    "name": ["Charlie", "David"],
    "age": [35, 40]
})

combined = pd.concat([df1, df2], ignore_index=True)
```

**Result of `concat()`:**

| name | age |
| --- | --- |
| Alice | 25 |
| Bob | 30 |
| Charlie | 35 |
| David | 40 |

Use `ignore_index=True` to reset the index after concatenation.

---

### 🎓 Want to Learn More?

Explore additional merge options and practice more examples at:

- [W3Schools - Pandas Merge](https://www.w3schools.com/python/pandas/ref_df_merge.asp)
- [W3 Resource - Pandas Concat](https://www.w3resource.com/pandas/concat.php)

These resources are a great place to strengthen your understanding of joining and combining data in Pandas!

---

🎉 **Recap:** In this SkillBuilder, you learned how to combine DataFrames in Pandas using different types of joins and concatenation. You practiced using `pd.merge()` to perform inner joins, which keep only matching rows from both DataFrames, and explored left joins to retain all rows from the left DataFrame while filling in `NaN` for missing matches. You also used `pd.concat()` to stack DataFrames vertically, similar to a SQL UNION ALL, combining rows into a single DataFrame. Throughout the lesson, you saw result tables for each join type to help you visualize how rows are matched or filled. If you'd like to explore further, be sure to check out the linked W3Schools tutorials for more examples and explanations of Pandas joins and concatenations!
