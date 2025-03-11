# MyCloset - Social Bookmarking Platform designed for clothes

- Web application implemented using ASP.NET Core and C# that represents a social bookmarking site for clothes, implemented along with a colleague.
- The app is tailored to allow users to view, add, like and comment on clothing articles. It features a main page with a search engine and a sorting system, ordering by date or popularity, which is determined by the number of likes each item has.
- Each user has a profile and they can create private or public collections with the items available on the platform.
- Designed and implemented backend logic, database interactions using Entity Framework, Dependency Injection, LINQ and SQL Server.
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

![Screenshot 2025-03-11 151255](https://github.com/user-attachments/assets/ebf44f6f-ba21-4bd3-9063-ba8efa250618)

- Each item features a title, a description and media content, in form of a picture. 

![Screenshot 2025-03-11 151357](https://github.com/user-attachments/assets/9026e7c9-2cb9-4a35-aa32-0c1764d0ea0a)

- Registered users can edit and delete their own items.
![Screenshot 2025-03-11 151131](https://github.com/user-attachments/assets/ce04a766-cc11-4490-8932-ec2b49316835)

- However, registered users cannot modify other users' items.

![Screenshot 2025-03-11 151057](https://github.com/user-attachments/assets/467f3097-dbb3-4f0a-a8b0-34ff9a314fec)

- Registered users are able to leave comments on any available item on the platform. Users can edit and delete strictly their own comments.

![Screenshot 2025-03-11 151144](https://github.com/user-attachments/assets/d437f990-af4f-411f-9cec-15c9d3a6260d)

![image](https://github.com/user-attachments/assets/7118e0f0-97a2-462b-8bca-938e5c756999)

- Registered users are allowed to cast a vote on every item on the platform, using a like system, users being able to remove a like on an arbitrary item. The like system was implemented using a many-to-many relationship between the entities UserLikes and Users: every user can like multiple items, and every item can be liked by multiple users.

![Screenshot 2025-03-11 151502](https://github.com/user-attachments/assets/ae1c04ed-09fd-46de-9323-5fef8641ed86)

- Each user can create their own collections, organising the available articles of clothing in a personalized fashion. These collections are public (visible on the user's profile page) or private (visible only to the owner of that certain collection).
![Screenshot 2025-03-11 235226](https://github.com/user-attachments/assets/b92b9eee-33c3-4aad-a593-be072e4aad4e)
- In this case, this absolutely gorgeous blouse is already added to the collection.
![Screenshot 2025-03-11 235240](https://github.com/user-attachments/assets/d2f6ad4a-6b7d-4a65-8ab3-62af64a86c78)
- Each user benefits from a personal profile page, containing their username, a profile picture, first name, last name, bio, and other relevant details. If that certain user has public collections, then they will be visible on the page.
- Viewing as `user@test.com` my own profile page:
![Screenshot 2025-03-11 151427](https://github.com/user-attachments/assets/95e14b55-0ad5-4196-9978-22a34983d371)
- Viewing another user's profile page:
![Screenshot 2025-03-11 151443](https://github.com/user-attachments/assets/04d96c64-4405-4e32-937e-41d225d7ca95)

- The index tab of the platform features a search engine, being able to search by title, description or possible public collections the searched items are in.
- Every item shown is in a public collection called "Favorite" and we can search for items using only chunks of words.
![image](https://github.com/user-attachments/assets/6d8ac764-1fb0-4bae-b62d-0e6f01291d5a)

### Administrator

- Admins have the responsibility of managing the platform, they have access to everything and they can remove any inappropiate content that may arise. They may delete items and comments, regardless if that content was posted by them or not.

![Screenshot 2025-03-11 151518](https://github.com/user-attachments/assets/5dda2b4b-b814-46d7-896c-c73bcb2e54a9)

![Screenshot 2025-03-11 151535](https://github.com/user-attachments/assets/9368ee13-09ed-400f-8097-7f0ba8dee709)





