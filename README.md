# Chatroom-Flask-React
**Mini Project (Group-5)**

**Topic: Chatroom (Flask + React)**

**Members : Dinesh Kumar, Vinay Chauhan, Prabhpreet Singh, Rohit Kashyap**

1. **What this project covers?**

- Responsive UI made with React
- Backend made with Flask
- JWT implementation
- Login &amp; Registration with relevant APIs
- Flask-SocketIO used for real time chatting. (Both group as well as one to one)
- Postgresql used for database

2. **To run this project locally follow the following documentation:**

- **Install node.js**
- **Open folder client**
- **npm install (This will install all node\_modules)**
- **npm start**

3. **To run backend**

- **create virtual environment**
- **Install requirement.txt**
- **create database chatroom in postgres**
- &quot;postgresql://postgres:root@localhost/chatroom&quot;
- **flask run**

4. **Run frontend and backend server separately.**

- If facing any issues clear the localStorage of browser.
- And login again.

5. **To check the group chat feature**

- Open two tabs one normally in browser and other in Incognito Mode.
- Register and after that Login with different account.
- Open group chat and start chatting simultaneously with different accounts.
- If facing any issues clear the localStorage of browser.
- And login again.

6. **To check the personal chat feature**

- Open two tabs one normally in browser and other in Incognito Mode.
- Register if not done and after that Login with different account.
- Open personal chat in both tabs normal and incognito and enter recipient&#39;s username in each other tab from registered user list displayed in left, start chatting simultaneously with different accounts.
- If facing any issues clear the localStorage of browser.
- And login again.

7. **If any issue occurs restart the backend server and frontend server as well.**
8. **APIs and SocketIO**

**/loginsuccess** method=POST
 Takes email and password and also do JWT authentication.
 
![Screenshot from 2021-12-13 04-23-07](https://user-images.githubusercontent.com/55187704/145733944-daa6e8b2-4a14-4d3b-a404-e2139c0f0a7d.png)

**/registrationsuccess** method=POST

Takes name, email and password and store data to database.

![Screenshot from 2021-12-13 04-23-22](https://user-images.githubusercontent.com/55187704/145733959-ce9b4b61-b034-49ac-984d-1ccaca19b43d.png)

**/user** method=GET

Send all registered users List to frontend.
 
![Screenshot from 2021-12-13 04-23-34](https://user-images.githubusercontent.com/55187704/145733967-49e426ab-6708-4ba5-96a1-7d20e61eb18e.png)

**/group** namespace used for group chat
 &#39;Message&#39; event listen request from client and broadcast it to others.

![Screenshot from 2021-12-13 04-23-51](https://user-images.githubusercontent.com/55187704/145733974-60384a8f-6661-4a0a-806d-7ad97ca21358.png)

**/private** namespace used for personal chat

&#39;username&#39; event stores the new added user to user dictionary with value request.sid

&#39;Private\_message&#39; event listen message and emit message to particular user session\_id.

![Screenshot from 2021-12-13 04-24-11](https://user-images.githubusercontent.com/55187704/145733910-b50df772-caa4-47c3-85a6-319abcabe11e.png)

1. **For Frontend Route and Switch used from React-router-dom for making various routes.**

![Screenshot from 2021-12-13 04-39-25](https://user-images.githubusercontent.com/55187704/145733892-30646fa1-d0f0-4a10-904c-47e18509e608.png)


**SCREENSHOTS of working project**

![Screenshot from 2021-12-13 02-35-38](https://user-images.githubusercontent.com/55187704/145733764-2414e5ee-36d2-402b-91f0-0bf34b9a11d8.png)
![Screenshot from 2021-12-13 02-35-47](https://user-images.githubusercontent.com/55187704/145733765-e460427e-64cf-442f-8f95-d29348b9f6c3.png)
![Screenshot from 2021-12-13 02-35-56](https://user-images.githubusercontent.com/55187704/145733766-c15d9558-7b46-4c38-ba41-d6308f6f65d4.png)
![Screenshot from 2021-12-13 02-36-09](https://user-images.githubusercontent.com/55187704/145733768-3899f8b6-7590-421a-ae3d-ee4e8f1326aa.png)
![Screenshot from 2021-12-13 02-36-25](https://user-images.githubusercontent.com/55187704/145733769-7a97db91-3aed-4441-8c85-406dc92e740f.png)
![Screenshot from 2021-12-13 02-36-34](https://user-images.githubusercontent.com/55187704/145733771-acbf3488-fcaa-4cdd-90c5-a35f49a1d337.png)
![Screenshot from 2021-12-13 02-37-00](https://user-images.githubusercontent.com/55187704/145733773-a9579522-a0bc-4f16-9619-d8bfb4bdfa2c.png)
![Screenshot from 2021-12-13 02-38-19](https://user-images.githubusercontent.com/55187704/145733777-31e3479e-8f7f-442f-9e26-d7daf784dbb5.png)
![Screenshot from 2021-12-13 02-38-29](https://user-images.githubusercontent.com/55187704/145733780-421494c6-6358-43b6-a121-778c66743d3f.png)
![Screenshot from 2021-12-13 02-40-25](https://user-images.githubusercontent.com/55187704/145733783-ea23cbf5-49e6-43c0-a198-3cd6137c1ffe.png)
