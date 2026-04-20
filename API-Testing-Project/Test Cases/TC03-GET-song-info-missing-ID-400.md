## Test Case: GET /api/song/{song_id}/info with missing song ID returns 400 Bad Request

### Objective
Verify that the API returns **400 Bad Request** when a user attempts to retrieve song information **without providing a song ID** in the request path.

-

### Preconditions
- Valid registered user  
- Valid Bearer token  
- Postman environment configured  
- Endpoint `GET /api/song/{song_id}/info` is available  

---

### Test Data
- `token` — valid Bearer token  
- `song_id` — *missing*  

---

### Steps
1. Send a **GET** request to `/api/song//info` (omit the song ID).  
2. Add a valid Bearer token in the **Authorization** header.  
3. Submit the request.  
4. Observe the response.

---

### Expected Result
- Response status: **400 Bad Request**  
- Response body contains an error message indicating the **song ID is missing**.  
- No song information is returned.

---

### Actual Result
- The request returned **400 Bad Request**.  
- The response body included an error message stating that the song ID was required and not provided.  
- No song information was displayed.

---

### Evidence
- Screenshot: **TC03 – Missing song ID → 400 Bad Request**
