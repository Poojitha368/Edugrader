# EduGrader

**Requirements for running the project:**

```
pip install -r requirements.txt
```
```

CREATE DATABASE edugrader;
USE edugrader;

CREATE TABLE user (
    id INT AUTO_INCREMENT PRIMARY KEY,
    username VARCHAR(50),
    password VARCHAR(50),
    email VARCHAR(50)
);


CREATE TABLE history (
    qno INT AUTO_INCREMENT PRIMARY KEY,
    question VARCHAR(1500),
    answer VARCHAR(1500),
    feedback VARCHAR(1500),
    marks INT,
    user_id INT,
    FOREIGN KEY (user_id) REFERENCES user(id)  -- foreign key constraint
);




```

![Homepage](https://github.com/user-attachments/assets/e4437aeb-cf46-461a-a9b4-0211d944b960)

#   E d u g r a d e r  
 