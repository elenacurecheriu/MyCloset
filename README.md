# MyCloset - Social Bookmarking Platform designed for clothes

- Web application implemented using ASP.NET Core and C# that represents a social bookmarking site for clothes, implemented along with a colleague.
- The app is tailored to allow users to view, add, like and comment on clothing articles. It features a main page with a search engine and a sorting system, ordering by date or popularity, which is determined by the number of likes each item has.
- Each user has a profile and they can create private or public collections with the items available on the platform.
- Designed and implemented backend logic, database interactions using Entity Framework, LINQ and SQL Server.
- Created a responsive front-end with HTML, CSS, JavaScript, Bootstrap and Razor Pages. Integrated authentication and authorization using Identity Framework for secure user management.

## General features:

- Three types of user roles: guest, registered users and administrators
- Item search engine by title, category and description
- User profile page, with profile picture, name, bio and saved items
- Each item has a title, 
- Paginated view
- Like system
- Main page with sorting system ordering by date added or popularity (i.e. number of likes each article has)\

## Role specific features:

### Guest

- Guests are able to browse the main page, viewing the platform's articles. They can also choose to sort the articles based on popularity or date added.

![Screenshot 2025-03-11 150537](https://github.com/user-attachments/assets/0fbe710e-677d-4596-9a02-a66488650665)
![Screenshot 2025-03-11 150547](https://github.com/user-attachments/assets/4fc172bf-a02b-49f6-883c-db03458bbd00)

- However, if a guest tries to view an article, they are redirected to the login page:

![image](https://github.com/user-attachments/assets/381d1d26-276b-4bfc-9d0b-a32c41cff5ff)

### Registered user

- Registered users can add items on the platform, using the ```Adauga item``` button:



