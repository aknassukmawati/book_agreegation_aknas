# book_agreegation_aknas
class Buku:
    def __init__(self, judul, penulis, harga):
        self.judul = judul
        self.penulis = penulis
        self.harga = harga


class Bookstore:
    def __init__(self, name):
        self.name = name
        self.books = []

    def add_book(self, book):
        self.books.append(book)

    def display_books(self):
        print(f"Selamat datang di {self.name}:")
        for book in self.books:
            print(f"Judul: {book.judul}")
            print(f"Penulis: {book.penulis}")
            print(f"Harga: ${book.harga}")
            print()



bookstore = Bookstore("Toko buku ky")

book1 = Buku("Laskar Pelangi", "Andrea Hirata", 25000)
bookstore.add_book(book1)
book2 = Buku("Bumi Manusia", "Pramoedya Ananta Toer", 30000)
bookstore.add_book(book2)


bookstore.display_books()
