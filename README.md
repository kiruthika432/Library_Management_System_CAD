# Library_Management_System_CAD
.
          Title: Readify
Target audience: Librariens
           Type: B2B
          Users: Students, staff, Aspirants, Business man, Book warm etc
       Timeline: 2 to 3 weeks
      Team size: 1
Features and Workflow:
                 1, Register page
                 2, Login page
                 3, Library details management - storage management
                 4, Add Daily news
                 5, Add books
                 6, Add users
                 7, Searching and filtering books
                 8, Book details page
                 9, Borrowing book with timeline
                 10, Return page with feedback
                 11, Library users/ members manage - user detail page
                 12, Fine amount for overdue books - payment and details

System Design
          1, Class RegistrationInfo:
                  -       firstName: String
                  -        lastName: String
                  -        mobileNo: Long / String
                  -         emailID: String
                  -        password: String
                  - confirmPassword: String
                  -        userName: String
                  -             DOB: String
.    
          2, Class Login:
                  - userName: String
                  - password: String
.                  
          3, Class Library:
                  -               ID: int
                  -             name: String
                  -         incharge: String
                  -         capacity: int
                  - storageStructure: 
                  -          address: String
                  -          phoneNo: Long / String
                  -     wifiPassword: String
                  -          emailId: String
                  -      openingTime: Date / Long
                  -      closingTime: Date / Long
.
          4, Class Book:
                  -             ID: String
                  -           name: String
                  -          genre: String
                  -         volume: byte
                  -  publishedYear: Int
                  -        authour: String
                  -     noOfCopies: byte
                  - availableCount: byte
                  -          price: String
.
          5, Class User:
                  -         name: String
                  -        email: String
                  -      phoneNo: String
                  -      address: String
                  - membersSince: String
                  -       status: String
.
          6, Class BookSearchandFilter:
                  -       title: String
                  -     authour: String
                  -    category: String
                  - isAvailable: boolean
.
          7, Class BookDetailsPage:
                  -              ID: long
                  -           title: String
                  -         authour: String
                  -            ISBN: String
                  -        category: String
                  -     description: String
                  -       publisher: String
                  -     totalCopies: int
                  - availableCopies: int
.
          8, Class Borrowing:
                  -     userID: long
                  -     bookID: long
                  -       date: long
                  -    dueDate: long
                  - returnDate: long
                  - returnedBy: String
                  -   feedback: String
.
          9, Class Fine:
                  - borrowingID: long
                  -      amount: double
                  -        paid: boolean
.
          10, Class Payment:
                  -        fineID: long
                  -        method: String
                  -        amount: double
                  - transactionID: String
                  -        paidAt: String
.
          11, Class News:
                  -     title: String
                  -   content: String
                  - createdBy: String
                  - createdAt: String
        
