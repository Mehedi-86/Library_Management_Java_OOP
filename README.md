
   <h1 align="center">📚 Library Management System</h1>
<p>A console-based Library Management System developed in Java using Object-Oriented Programming (OOP) concepts.</p>

<h2>📖 Introduction</h2>
It provides an intuitive interface for users to sign up, log in, borrow books, return books, and track borrowed books. 
The system enforces borrowing limits, calculates late return fees, and allows users to view upcoming book returns.</p>

<h2>🚀 Features</h2>
<ul>
    <li>✅ <strong>Student Sign-Up & Login</strong> - Secure authentication using roll number and password.</li>
    <li>✅ <strong>View Available Books</strong> - Lists books that are currently available for borrowing.</li>
    <li>✅ <strong>View Borrowed Books</strong> - Displays books borrowed by a logged-in student.</li>
    <li>✅ <strong>Borrow a Book</strong> - Students can borrow up to 3 books at a time.</li>
    <li>✅ <strong>Return a Book</strong> - Return a borrowed book to the library.</li>
    <li>✅ <strong>View Late Return Fee</strong> - 2 TK per day fine for overdue books.</li>
    <li>✅ <strong>View Upcoming Books</strong> - Shows books due for return within the next 7 days.</li>
    <li>✅ <strong>Exit</strong> - Logout and exit the system.</li>
</ul>

<h2>📂 Project Structure</h2>
<pre>
Library_Management/
├── 📜 LibraryManagementSystem.java   # Main class for user interaction
├── 📜 Library.java                   # Manages books and student records
├── 📜 Book.java                      # Book entity with attributes and methods
├── 📜 Student.java                   # Student entity for handling authentication and borrowed books
├── 📜 OutPut.txt                     # Show the Functionality as Output Formate
├── 📜 README.md                      # Documentation file
</pre>

<h2>🛠 Class Structure</h2>

<h3>📘 Book Class</h3>
<pre>
- title (String)
- author (String)
- isBorrowed (boolean)
- dueDate (LocalDate)
+ getTitle(): String
+ getAuthor(): String
+ isBorrowed(): boolean
+ borrowBook(): void
+ returnBook(): void
+ getDueDate(): LocalDate
</pre>

<h3>👨‍🎓 Student Class</h3>
<pre>
- name (String)
- rollNumber (String)
- password (String)
- borrowedBooks (List<Book>)
+ getName(): String
+ getRollNumber(): String
+ verifyPassword(String): boolean
+ getBorrowedBooks(): List<Book>
+ borrowBook(Book): boolean
+ returnBook(Book): boolean
</pre>

<h3>🏛 Library Class</h3>
<pre>
- books (List<Book>)
- students (Map<String, Student>)
+ Library()
+ signUpStudent(String, String, String): void
+ loginStudent(String, String): Student
+ displayAvailableBooks(): void
+ viewBorrowedBooks(Student): void
+ viewUpcomingBooks(): void
+ borrowBook(Student, String): void
+ returnBook(Student, String): void
</pre>

<h3>📌 LibraryManagementSystem (Main Class)</h3>
<pre>
- main(String[]): void  // Handles user input and system flow
</pre>

<h2>💻 How to Run</h2>
<h3>🔹 Clone the Repository</h3>
<pre>
git clone https://github.com/Mehedi-86/Library_Management.git
cd Library_Management
</pre>

<h3>🔹 Compile and Run</h3>
<pre>
javac LibraryManagementSystem.java
java LibraryManagementSystem
</pre>

<h2>🛠 Future Enhancements</h2>
<ul>
    <li>✅ Implement graphical user interface (GUI) for better usability.</li>
    <li>✅ Add database integration for persistent storage.</li>
    <li>✅ Improve authentication system with encryption.</li>
    <li>✅ Implement book reservation and request system.</li>
</ul>

<h2>📜 License</h2>
<p>This project is open-source and available for modification and distribution under the MIT License.</p>

<h2>🎯 Conclusion</h2>
<p>The Library Management System is a simple yet effective solution for managing books and student interactions in a library. With features such as secure authentication, book borrowing and returning, and late fee tracking, it provides an essential framework for digitalizing library operations. Future enhancements, including GUI implementation and database integration, will further improve usability and efficiency. This project serves as a strong foundation for further development in library automation.</p>
