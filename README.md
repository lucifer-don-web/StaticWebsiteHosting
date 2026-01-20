# Simple Static Website Using AWS S3
A simple, highly available static website hosted on **Amazon S3**. This project demonstrates how to configure an S3 bucket to serve HTML and CSS content to the public internet without managing a traditional server.

## Key Features
- **Serverless:** No EC2 or servers needed  
- **Highly Available:** Uses AWS S3 infrastructure  
- **Public Access:** Configured bucket policy for global reach  

## Tech Stack
- **Frontend:** HTML5, CSS3  
- **Storage:** Amazon S3  
- **Security:** IAM & Bucket Policies  

## Project Configuration

### Bucket Setup
- **Bucket Name:** `static-web-op`  
- **Region:** `us-east-1 (N. Virginia)` 
<img width="624" height="243" alt="image" src="https://github.com/user-attachments/assets/2a11d4e8-1ae4-4fbc-9c4a-a7d341499e34" />


- **Public Access:** All "Block Public Access" settings were turned OFF to allow website access.

  <img width="624" height="244" alt="image" src="https://github.com/user-attachments/assets/18567ba8-d9bb-4002-8978-1621f5374e44" />


### File Structure
The following files were uploaded to the root directory of the bucket:  
- `index.html` – The main landing page  
- `style.css` – Contains the styling for the page layout  

<img width="624" height="154" alt="image" src="https://github.com/user-attachments/assets/351afe3f-45fb-4bc3-94f1-f653ac2fe139" />


### Website Hosting Configuration
- **Static Website Hosting:** Enabled  
- **Index Document:** `index.html`  

<img width="624" height="245" alt="image" src="https://github.com/user-attachments/assets/a2889b6c-3418-48fe-a533-0b5b69a5d55b" />

### Permissions (Bucket Policy)
To allow public read access, the following JSON policy was applied to the bucket:

<img width="460" height="272" alt="image" src="https://github.com/user-attachments/assets/295ef38a-0baf-49a5-9a56-2b32fe95730d" />

### Access The Website
   The website can be accessed using the S3 bucket website endpoint URL, such as:
      http://static-web-op.s3-website-us-east-1.amazonaws.com

<img width="624" height="287" alt="image" src="https://github.com/user-attachments/assets/ba354f3b-6721-43b1-bd3f-40acd901a8dd" />

### Learning & Challenges

- **Learned:** How to configure S3 bucket policies for public access.
- **Gained experience:** Hosting static websites without a server.
- **Challenge:** Understanding IAM permissions and ensuring the website was publicly accessible.

### Author

**Kishan Deep Lamichhane**  
GitHub: https://github.com/Kishandeeplamichhane



