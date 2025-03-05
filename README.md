# Saylani Final Test Paper

This project is a **Python Final Test** submission for Saylani, covering two tasks:
1. File Analysis and Word Search.
2. Library Management System using Object-Oriented Programming (OOP).

---

## 1. File Analysis and Word Search

### Description
The **File Analysis System** reads a file and performs the following operations:
- Count the number of characters, words, and lines in the file.
- Search for the occurrences of a specific word.

### Features
- Error Handling for Missing Files.
- Word Search Functionality.
- Accurate Character, Word, and Line Count.

### Functions
#### `analyze_file(file_name)`
- Reads the file.
- Returns a dictionary containing:
    - Characters count.
    - Words count.
    - Lines count.

#### `search_word(file_name, word)`
- Reads the file.
- Returns the count of a specific word in the file.

### Example Output
```python
File Analysis: {'characters': 55, 'words': 12, 'lines': 1}
The word 'Python' occurs 0 times in the file.
```

---

## 2. Library Management System (OOP)

### Description
The **Library Management System** manages books, users, and borrowing transactions. The system includes physical, digital, and audiobook types.

### Classes
- `Book`: Base class for books.
- `DigitalBook`: Inherits from `Book` with an additional `file_format` attribute.
- `AudioBook`: Inherits from `Book` with an additional `duration` attribute.
- `User`: Represents users borrowing books.
- `Library`: Manages books and users.

### Features
- Book Borrowing and Returning.
- Digital and Audiobook Support.
- User Registration.
- Encapsulation with private attributes.

### Example Usage
```python
library = Library("City Karachi Library")

book1 = Book("2024", "harrypotter_byharis", 1222, "112233")
digital_book = DigitalBook("Learn Python", "fromyasir", 2023, "mola", "PDF")
audio_book = AudioBook("story of harry", "princes", 2019, "12131", 12.5)

library.add_book(book1)
library.add_book(digital_book)
library.add_book(audio_book)

user1 = User("user01", "abubakar")
library.register_user(user1)
library.lend_book("user01", "112233")
library.receive_return("user01", "112233")
```

### Output
```python
Added '2024' to the library.
Registered user: abubakar (ID: user01)
You have borrowed '2024'.
You have returned '2024'.
```

---

### Technologies Used
- Python
- Object-Oriented Programming (OOP)

### Author
**M Haris Chaudhary**

### Special Thanks
- Saylani Welfare Trust
- Sir Qasim

---

### License
This project is for educational purposes only.

