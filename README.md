# -Book_Agreegation_Tias
class Book:
    def __init__(self, title, author, price):
        self.title = title
        self.author = author
        self.price = price


class Bookstore:
    def __init__(self, name):
        self.name = name
        self.books = []

    def add_book(self, book):
        self.books.append(book)

    def display_books(self):
        print(f"Buku yang tersedia di{self.name}:")
        for book in self.books:
            print(f"Judul: {book.title}")
            print(f"Pengarang: {book.author}")
            print(f"Harga: {book.price}")
            print()


# Create Book objects
book1 = Book("Python Crash Course", "Eric Matthes", 29.99)
book2 = Book("The Pragmatic Programmer", "Andrew Hunt, David Thomas", 49.99)
book3 = Book("Clean Code", "Robert C. Martin", 39.99)

# Create Bookstore object
bookstore = Bookstore("Toko Buku Tias")

# Add books to the Bookstore
bookstore.add_book(book1)
bookstore.add_book(book2)
bookstore.add_book(book3)

# Display the available books
bookstore.display_books()
