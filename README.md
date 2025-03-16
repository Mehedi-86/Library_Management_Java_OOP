<h2>📌 Features</h2>
<ul>
    <li><strong>Student Sign-Up & Login</strong> - Secure authentication using roll number and password.</li>
    <li><strong>View Available Books</strong> - Lists books that are currently available for borrowing.</li>
    <li><strong>View Borrowed Books</strong> - Displays books borrowed by a logged-in student.</li>
    <li><strong>Borrow a Book</strong> - Students can borrow up to 3 books at a time.</li>
    <li><strong>Return a Book</strong> - Return a borrowed book to the library.</li>
    <li><strong>View Late Return Fee</strong> - 2 TK per day fine for overdue books.</li>
    <li><strong>View Upcoming Books</strong> - Shows books due for return within the next 7 days.</li>
    <li><strong>Exit</strong> - Logout and exit the system.</li>
</ul>

<h2>📂 Project Structure</h2>
<pre>
Library_Management/
├── LibraryManagementSystem.java (Main class for user interaction)
├── Library.java (Manages books and student records)
├── Book.java (Book entity with attributes and methods)
├── Student.java (Student entity for handling authentication and borrowed books)
├── README.md (This file)
</pre>

<h2>🛠 Class Structure</h2>

<h3>1. Book Class</h3>
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

<h3>2. Student Class</h3>
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

<h3>3. Library Class</h3>
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

<h3>4. LibraryManagementSystem (Main Class)</h3>
<pre>
- main(String[]): void  // Handles user input and system flow
</pre>

<h2>🚀 How to Run</h2>
<pre>
1. Open terminal and navigate to project folder: 
   <code>cd /path/to/Library_Management</code>
2. Compile the Java files: 
   <code>javac LibraryManagementSystem.java</code>
3. Run the program: 
   <code>java LibraryManagementSystem</code>
</pre>

<h2>📜 License</h2>
<p>This project is open-source and available for modification and distribution.</p>
