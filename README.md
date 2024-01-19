# Instagram Clone Project - SQL Queries

## Overview

This project centers around building an Instagram Clone with a specific emphasis on designing and implementing SQL queries for efficient data retrieval, manipulation, and management. The goal is to create a robust database structure and optimize queries to ensure smooth performance for a social media platform.

## Features

- **User Management:** SQL queries for user registration, login, profile updates, and authentication.
- **Photo Sharing:** Efficient storage and retrieval of image data, handling captions, and associated metadata.
- **Followers/Following:** SQL queries to manage user relationships, including following and unfollowing.
- **Feed Optimization:** Designing queries for generating personalized feeds based on user-following relationships.
- **Likes and Comments:** Managing likes and comments with SQL queries for insertion, retrieval, and updates.

## Database Schema

The database design is crucial for optimizing SQL queries. Here's a simplified schema:

### Tables

1. **Users**
   - UserID (Primary Key)
   - Username
   - Email
   - Password (Hashed)
   - Profile Picture
   - ...

2. **Posts**
   - PostID (Primary Key)
   - UserID (Foreign Key to Users)
   - Image
   - Caption
   - LikesCount
   - ...

3. **Followers**
   - FollowerID (Primary Key)
   - FollowerUserID (Foreign Key to Users)
   - FollowingUserID (Foreign Key to Users)
   - ...

4. **Comments**
   - CommentID (Primary Key)
   - PostID (Foreign Key to Posts)
   - UserID (Foreign Key to Users)
   - Text
   - ...

## SQL Query Examples

1. **Retrieve User's Posts:**
   ```sql
   SELECT * FROM Posts WHERE UserID = :userID;
