# <img src="https://cloud.githubusercontent.com/assets/7833470/10899314/63829980-8188-11e5-8cdd-4ded5bcb6e36.png" height="60"> Project Vagabond: User Stories

**Elevator Pitch:** A travel community for users to share city-specific tips ("posts" or "logs") about their favorite locations around the world.

---

## Sprint 1: Homepage

**A user should be able to:**

1. Navigate to "/" and see a basic splash page with:
  * The name of the website.

---

## Sprint 2: CRUD

**A user should be able to:**

1. Link to other pages from homepage.
1. View the "San Francisco" page (at "/cities/1") including:
  * The site-wide header.
  * The name of the city.
  * An iconic photo of the city.
1. View a list of posts on the San Francisco page:
  * Sorted by newest first.
  * With the post titles linked to the individual post "show" pages.
1. Use an "Add New Post" button on the San Francisco city page to pull up the new post form.
1. Create a new post for San Francisco (**Hint:** <a href="http://guides.rubyonrails.org/routing.html#nested-resources" target="_blank">nested resources</a>).
1. Click "Edit" on ANY individual post, and be redirected to the edit form.
1. Click "Delete" on ANY individual post, then:
  * See a pop-up that says: "Are you sure you want to delete #{title}?"
  * If the user confirms, delete the post.

### Bonuses

**A user should be able to:**

1. Visit city pages via pretty urls, like "/cities/san-francisco".
  * Check out https://github.com/norman/friendly_id
1. On a city's page:
  * See post content truncated to 1000 characters max, with a link to view more.
  * See a relative published date, e.g. "2 days ago".

---

## Sprint 3: Validations

**A user should be able to:**

1. View city pages for "London" and "Gibraltar".
1. Verify that a new post they create is successfully published on the correct city page.

A user CANNOT save invalid data to the database, according to the following rules:

1. A post's title must be between 1 and 200 characters.
1. A post's content must not be empty.

#### Bonuses

**A user should be able to:**

1. View an error message when form validations fail, for the following validations:
  * Title must be between 1 and 200 characters.
  * Content must not be empty.
1. View only the 10 most recent posts on a city page (pagination), with
  * A link/button to the "Next" 10.
  * A link/button to the "Previous" 10.
1. See a list of the city pages they've contributed to, on their public profile
1. See the number of posts they've written for each city, next to the city's name in their profile.
1. View all vagabond cities as markers/pins on a map on the site's homepage.
1. Click on a pin on the homepage map and be redirected to the corresponding city page.

---

## Sprint 4: Commenting
1. Comment your code!!!
  * This will help you later when you come back to your code, or help you explain to potential employers how your code works.

### Bonuses

**A user should be able to:**

1. Comment on individual posts.
1. See the number of comments a post has on the post's "show" page.
1. See the number of comments they've left, on their public profile.
