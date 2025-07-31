

# Library Management System (SQL Project)

This project is a fully functional **Library Management System** built using **Microsoft SQL Server** and **T-SQL stored procedures**. It demonstrates how to create a normalized database schema for a library and perform complex queries using stored procedures.

## Project Structure

- **Database Creation**: Creates `db_LibraryManagement` with multiple related tables.
- **Tables**:
  - `tbl_publisher`
  - `tbl_book`
  - `tbl_library_branch`
  - `tbl_borrower`
  - `tbl_book_loans`
  - `tbl_book_copies`
  - `tbl_book_authors`
- **Data Insertion**: Preloaded sample data for publishers, books, branches, borrowers, loans, and more.
- **Stored Procedures**: Includes common and advanced queries as reusable procedures.

## Features

- 📖 Track books, authors, and publishers
- 🏬 Manage multiple library branches
- 👤 Handle borrower records
- 📄 Record book loans and due dates
- 📊 Generate custom reports using stored procedures

## Technologies Used

- Microsoft SQL Server
- T-SQL (Transact-SQL)
- Stored Procedures
- JOINs, Aggregations, Subqueries

## Sample Stored Procedures

| Procedure Name                | Description |
|------------------------------|-------------|
| `bookCopiesAtAllSharpstown`  | Find number of copies of a specific book at Sharpstown branch |
| `bookCopiesAtAllBranches`    | Get copies of a book across all branches |
| `NoLoans`                    | List borrowers with no books checked out |
| `LoanersInfo`                | List borrowers with books due today at a specific branch |
| `TotalLoansPerBranch`        | Count total loans per branch |
| `BooksLoanedOut`             | Borrowers with more than 5 books checked out |
| `BookbyAuthorandBranch`      | Find books by a certain author at a specific branch |

## How to Run

1. Open SQL Server Management Studio (SSMS).
2. Copy and run the full script in the query window.
3. Execute any of the stored procedures at the bottom of the script to view results.

## Example Execution

```sql
EXEC dbo.bookCopiesAtAllSharpstown;
EXEC dbo.BooksLoanedOut;

