Personal Library
================

Build a full stack JavaScript app that is functionally similar to this: [https://personal-library.freecodecamp.rocks/](https://personal-library.freecodecamp.rocks/). Working on this project will involve you writing your code using one of the following methods:

*   Clone [this GitHub repo](https://github.com/freeCodeCamp/boilerplate-project-library) and complete your project locally.
*   Use [our Gitpod starter project](https://gitpod.io/?autostart=true#https://github.com/freeCodeCamp/boilerplate-project-library) to complete your project. Learn [how to share your Gitpod workspace to get help](https://forum.freecodecamp.org/t/how-to-use-gitpod-in-the-curriculum/668669#how-can-i-share-my-workspace-to-get-help-8).
*   Use a site builder of your choice to complete the project. Be sure to incorporate all the files from our GitHub repo.

* * *

1.  Add your MongoDB connection string to `.env` without quotes as `DB` Example: `DB=mongodb://admin:pass@1234.mlab.com:1234/fccpersonallib`
2.  In your `.env` file set `NODE_ENV` to `test`, without quotes
3.  You need to create all routes within `routes/api.js`
4.  You will create all functional tests in `tests/2_functional-tests.js`

Tests
-----

1\. You can provide your own project, not the example URL.

2\. You can send a **POST** request to `/api/books` with `title` as part of the form data to add a book. The returned response will be an object with the `title` and a unique `_id` as keys. If `title` is not included in the request, the returned response should be the string `missing required field title`.

3\. You can send a **GET** request to `/api/books` and receive a JSON response representing all the books. The JSON response will be an array of objects with each object (book) containing `title`, `_id`, and `commentcount` properties.

4\. You can send a **GET** request to `/api/books/{_id}` to retrieve a single object of a book containing the properties `title`, `_id`, and a `comments` array (empty array if no comments present). If no book is found, return the string `no book exists`.

5\. You can send a **POST** request containing `comment` as the form body data to `/api/books/{_id}` to add a comment to a book. The returned response will be the books object similar to **GET** `/api/books/{_id}` request in an earlier test. If `comment` is not included in the request, return the string `missing required field comment`. If no book is found, return the string `no book exists`.

6\. You can send a **DELETE** request to `/api/books/{_id}` to delete a book from the collection. The returned response will be the string `delete successful` if successful. If no book is found, return the string `no book exists`.

7\. You can send a **DELETE** request to `/api/books` to delete all books in the database. The returned response will be the string `complete delete successful` if successful.

8\. All 10 functional tests required are complete and passing.