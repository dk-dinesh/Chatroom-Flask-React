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

![](RackMultipart20211212-4-15q44om_html_8648364dea4df585.png)

**/registrationsuccess** method=POST

Takes name, email and password and store data to database.

![](RackMultipart20211212-4-15q44om_html_7fa55dbe782995cb.png)

**/user** method=GET

Send all registered users List to frontend.
 ![](RackMultipart20211212-4-15q44om_html_d8e8ede4c62fd046.png)

**/group** namespace used for group chat
 &#39;Message&#39; event listen request from client and broadcast it to others.

![](RackMultipart20211212-4-15q44om_html_9cd11eb5d3575add.png)

**/private** namespace used for personal chat

&#39;username&#39; event stores the new added user to user dictionary with value request.sid

&#39;Private\_message&#39; event listen message and emit message to particular user session\_id.

![](RackMultipart20211212-4-15q44om_html_c59c79551450cef3.png)

1. **For Frontend \&lt;Route\&gt; and \&lt;Switch\&gt; used from React-router-dom for making various routes.**

![](RackMultipart20211212-4-15q44om_html_5733b067d0fe2cf5.png)

**SCREENSHOTS of working project**

![](RackMultipart20211212-4-15q44om_html_213951998c22c154.png) ![](RackMultipart20211212-4-15q44om_html_262d21bec8eb6c93.png) 
![](RackMultipart20211212-4-15q44om_html_f16a212dbd6a8ac.png) ![](RackMultipart20211212-4-15q44om_html_74199c1cc5491909.png) 
![](RackMultipart20211212-4-15q44om_html_cff6eac4a14f5281.png) ![](RackMultipart20211212-4-15q44om_html_fec9862f30128081.png) 
![](RackMultipart20211212-4-15q44om_html_8d0a425b85be9155.png) ![](RackMultipart20211212-4-15q44om_html_65edc1a4dc7a53df.png) 
![](RackMultipart20211212-4-15q44om_html_552beb389d0aa12e.png) ![](RackMultipart20211212-4-15q44om_html_3197064634861d5f.png)
