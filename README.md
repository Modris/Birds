# Bird website ziniputnu.lv 

![Home Page](/project_images/mainpage_img.png)
* Discover 40 common bird species in Latvia.
  
* Test your knowledge in a memory game. 40 species. 160 images.

* Responsive web design. From mobile phones,tablets and computers - the website is functional.

* Mobile first approach. Mobile has compressed and resized wepb images for faster image loading. 
  
* No page reloads! Single Page Application with Vue.js means no page refreshes to navigate between links leads to a better user experience. 
  
# Small Demo link: Click image to be redirected to youtube.

[![Video Demo](/project_images/video_thumbnail.png)](https://www.youtube.com/watch?v=Lb6HCQEuklg)


# The tech stack. Main takeaways:

* Backend: Spring Boot, Spring Data JPA, MySQL
* Frontend: Vue.js
* Both are containerized with Docker into a Dockerfile. Deploy anywhere.

# Backend API 

| Endpoint                    | HTTP Method | Request Body | Status | Response Body | Description                                         |
| --------------------------- | ----------- | ------------ | ------ | -------------- | --------------------------------------------------- |
| /birds                      | GET         |              | 200    | List<Bird>     | Fetch all 40 birds with all categories and location data in JSON.               |
| /birds                      | GET         |              | 204    |                | No birds data in the database. Should not happen.                                |
| /birds/{id}                 | GET         | Bird         | 200    | Bird           | Fetch data about a specific bird with all categories and locations data in JSON. |
| /birds/{id}                 | GET         | Bird         | 204    |                | No bird with such ID. As of now, we have birds 1-40 available.                  |
| /details/{id}               | GET         | Details      | 200    | Details        | Fetch details data with this ID. As of now, details have ID's from 1-240.       |
| /details/{id}               | GET         | Details      | 204    |                | No details with such ID.                                                          |
| /details/birds/{birdsId}    | GET         | String       | 200    |                | Fetch details for a specific bird. Each bird usually has 6 details.             |
| /details/birds/{birdsId}    | GET         | String       | 204    |                | No details for such bird. As of now, available bird IDs are 1-40.                |

# Project images:


![Bird](/project_images/putns.png)

# Set Up

* Please check backend and frontend repositories respectively to see more specific project information. This is just broad overview.
