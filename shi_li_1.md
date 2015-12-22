# 示例1

**Title**
----


* **URL**


* **Method:**
  
  `GET` | `POST` | `DELETE` | `PUT`
  
*  **URL Params**


*   **Required:**
 
   `id=[integer]`

*   **Optional:**
 
   `photo_id=[alphanumeric]`

* **Data Params**


* **Success Response:**
  

  * **Code:** 200 <br />
    **Content:** `{ id : 12 }`
 
* **Error Response:**


  * **Code:** 401 UNAUTHORIZED <br />
    **Content:** `{ error : "Log in" }`

  OR

  * **Code:** 422 UNPROCESSABLE ENTRY <br />
    **Content:** `{ error : "Email Invalid" }`

* **Sample Call:**


* **Notes:**